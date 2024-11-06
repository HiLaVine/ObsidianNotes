Configuraciones
- springdoc.api-docs.enable=true
- springdoc.swagger-docs.enable=true

proyecto frases


spring.application.name=FrasesAPI

server.port=8484

spring.datasource.url=jdbc:mysql://localhost:3306/Frases
spring.datasource.username=root
spring.datasource.password=Fantasma1
spring.jpa.database-platform=org.hibernate.dialect.MySQLDialect

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
logging.level.org.hibernate.SQL=debug

spring.jpa.hibernate.naming.physical-strategy=org.hibernate.boot.model.naming.PhysicalNamingStrategyStandardImpl
spring.jpa.hibernate.naming.implicit-strategy=org.hibernate.boot.model.naming.ImplicitNamingStrategyLegacyJpaImpl

********************************************************************
package com.ipn.mx.domain.entidades;

import jakarta.persistence.*;
import lombok.AllArgsConstructor;
import lombok.Builder;
import lombok.Data;
import lombok.NoArgsConstructor;

import java.io.Serializable;

@Data
@NoArgsConstructor
@AllArgsConstructor
@Builder
@Entity
@Table(name = "Frase")
public class Frase implements Serializable {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    @Column(name = "idFrase", nullable = false)
    private Long idFrase;
    @Column(name = "texto", length = 500, nullable = false)
    private String texto;
    @Column(name = "autor", length = 100, nullable = false)
    private String autor;

}

********************************************************************

package com.ipn.mx.domain.repositorios;

import com.ipn.mx.domain.entidades.Frase;
import org.springframework.data.jpa.repository.JpaRepository;
import org.springframework.data.repository.CrudRepository;

public interface FraseRepository extends CrudRepository<Frase, Long> {

}
********************************************************************
package com.ipn.mx.service;

import com.ipn.mx.domain.entidades.Frase;

import java.util.List;

public interface FraseService {
    public List<Frase> listar();
    public Frase buscarId(Long id);
    public Frase guardar(Frase frase);
    public void delete(Long id);

    public Frase mostrarFraseAleatoria(List<Frase> listaDeFrases);

}

********************************************************************
package com.ipn.mx.service.impl;

import com.ipn.mx.domain.entidades.Frase;
import com.ipn.mx.domain.repositorios.FraseRepository;
import com.ipn.mx.service.FraseService;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Service;
import org.springframework.transaction.annotation.Transactional;

import java.util.List;

@Service
public class FraseServiceImpl implements FraseService {
    @Autowired
    FraseRepository dao;
    @Override
    @Transactional(readOnly = true)
    public List<Frase> listar() {
        return (List<Frase>) dao.findAll();
    }

    @Override
    @Transactional
    public Frase buscarId(Long id) {
        return dao.findById(id).orElse(null);
    }

    @Override
    @Transactional
    public Frase guardar(Frase frase) {
        return dao.save(frase);
    }

    @Override
    @Transactional
    public void delete(Long id) {
        dao.deleteById(id);
    }

    @Override
    @Transactional(readOnly = true)
    public Frase mostrarFraseAleatoria(List<Frase> listaDeFrases) {
        //mostrar una frase aleatoria del conjunto de frases existentes
        return null;
    }
}
********************************************************************

package com.ipn.mx.controlller;

import com.ipn.mx.domain.entidades.Frase;
import com.ipn.mx.service.FraseService;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.http.HttpStatus;
import org.springframework.web.bind.annotation.*;

import java.util.List;

@RestController
@RequestMapping("/api/ver1/frases")
@CrossOrigin(origins = {"*"})
public class FraseController {
    @Autowired
    FraseService service;
    @GetMapping("/frases")
    public List<Frase> listar() {
        return service.listar();
    }

    //localhost:8484/api/ver1/frases/frases/3
    @GetMapping("/frases/{id}")
    public Frase buscar(@PathVariable Long id) {
        return service.buscarId(id);
    }

    //localhost:8484/api/ver1/frases/frases
    @PostMapping("/frases")
    @ResponseStatus(HttpStatus.CREATED)
    public Frase crearFrase(@RequestBody Frase frase) {
        return service.guardar(frase);
    }

    //localhost:8484/api/ver1/frases/frases/3
    @PutMapping("/frases/{id}")
    @ResponseStatus(HttpStatus.CREATED)
    public Frase actualizarFrase(@RequestBody Frase frase,
                                 @PathVariable Long id) {
        Frase f = service.buscarId(id);
        f.setTexto(frase.getTexto());
        f.setAutor(frase.getAutor());

        return service.guardar(f);
    }

    @DeleteMapping("/frases/{id}")
    @ResponseStatus(HttpStatus.NO_CONTENT)
    public void eliminar(@PathVariable Long id) {
        service.delete(id);
    }

    @GetMapping("/frases/aleatorio")
    public Frase mostrarAleatorio() {
        return service.mostrarFraseAleatoria(service.listar());
    }

}


Rest controller

requestMaping(" eso es donde van los asteriscos")