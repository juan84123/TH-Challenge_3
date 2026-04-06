1️⃣ Escenario y Desafío ❄️

Después de reconstruir la comunicación mundial con sockets, pensaste que el caos había terminado.
Error.

Los mensajes ahora fluyen, pero el sistema comercial de la colonia empezó a fallar:
    Pedidos que cambian de estado sin explicación
    Pagos que no aparecen cuando alguien los reclama
    Auditorías que preguntan: “¿Quién modificó esto y cuándo?”

Un mensaje aparece en la consola:
    “Persistir no es guardar datos. Es poder defenderlos.”

La Academia exportó todo a archivos CSV. Datos crudos. Sin garantías. Sin integridad. Tu misión ya no es comunicar sistemas. Es construir el núcleo transaccional real de Penguin Academy.

Tenés 1 semana. Tu herramienta: SQL.
2️⃣ Objetivo del Challenge 🎯

Construir una base de datos relacional funcional que permita:
    Crear las tablas necesarias a partir del dominio implícito en los CSV
    Insertar los datos respetando reglas de integridad
    Definir relaciones mediante PK y FK
    Consultar la información de forma coherente
    Detectar inconsistencias estructurales usando SQL

No se evalúa solo que funcione. Se evalúa si el diseño tiene criterio y se puede defender.
3️⃣ Habilidades que vas a tener que invocar 🧠
    📥 Importación ordenada desde CSV
    🧱 Modelado relacional
    🔐 PK, FK, NOT NULL y CHECK
    📖 SELECT + JOIN + WHERE + ORDER BY
    🕵️ Detección de inconsistencias estructurales
    ⚡ Indexación básica
    🔒 Comprensión de SQL Injection

4️⃣ Motor de Base de Datos 🗄️
Podés usar cualquier motor relacional:
    SQLite
    PostgreSQL
    MySQL / MariaDB
    SQL Server
    Otro motor relacional equivalente

Condición obligatoria:
Debés justificar técnicamente tu elección explicando:
    Ventajas en este contexto
    Manejo de integridad referencial
    Soporte para constraints e índices
    Comportamiento ante carga desde CSV
    Limitaciones relevantes

Elegir tecnología también es diseñar.
5️⃣ Requisitos Obligatorios ✅
5.1 Creación del Modelo y Tablas

A partir exclusivamente del análisis de los CSV provistos.
Que los encontras en: https://drive.google.com/file/d/165buK18daMtHj_3xpRLin5cVdVsNiMRB/view?usp=sharing, debés:

    Identificar las entidades necesarias
    Inferir el significado de cada campo
    Crear tus propias tablas
    Definir tipos de datos adecuados
    Establecer claves primarias
    Definir y justificar relaciones

No se provee una lista de tablas mínimas. No se provee descripción de campos. El modelo surge del análisis del dominio. Si necesitás que alguien te explique qué representa una columna, tu modelo todavía no es tuyo.
5.2 Inserción de Datos

Debés:

    Insertar los datos desde los CSV
    Respetar el orden lógico de inserción
    Permitir que las violaciones de integridad fallen

Si todo entra sin errores, el diseño es débil.
5.3 Integridad y Restricciones

El modelo debe incluir, cuando corresponda:

    Claves primarias reales
    Claves foráneas reales
    NOT NULL coherentes
    CHECK para evitar valores inválidos
    UNIQUE cuando el dominio lo requiera
    Índices en columnas críticas

Nada decorativo. Todo defendible.
5.4 Consultas Estructurales (sin agregaciones)

Las consultas deben permitir:

    Navegar el modelo
    Relacionar entidades
    Rastrear estados y eventos
    Detectar ausencias

Solo se permite usar: SELECT, JOIN, WHERE, ORDER BY.
No se permiten: GROUP BY, Funciones de agregación.
El foco es estructura y diseño, no métricas.
5.5 Validación de Integridad

Debés construir consultas que detecten:

    Relaciones rotas
    Valores inválidos
    Entidades incompletas
    Estados imposibles
    Registros inconsistentes

La base debe poder señalar sus propias fallas.
5.6 Seguridad – SQL Injection 🔒

Debés explicar claramente:

    Cómo ocurre una SQL Injection
    Qué práctica la habilita
    Qué consecuencias puede tener
    Cómo debe diseñarse correctamente el acceso a datos
    Qué cambia al usar consultas parametrizadas

No respuestas superficiales.
6️⃣ Bonus XP 🎁

    Comparación de performance con y sin índices
    Dockerización del entorno
    Reglas fuertes a nivel de modelo
