# Gestor-de-Pedidos-DB
# 📦 Gestor de Pedidos - Base de Datos

Solución completa de base de datos para el sistema de gestión de pedidos, incluyendo esquema, datos iniciales, funciones, triggers y migraciones controladas con **Liquibase**.

## 📋 Tabla de Contenidos

- [Descripción](#-descripción)
- [Requisitos Previos](#-requisitos-previos)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Instalación](#-instalación)
- [Migraciones](#-migraciones)
- [Esquema de Base de Datos](#-esquema-de-base-de-datos)
- [Contribución](#-contribución)

## 🎯 Descripción

Este repositorio contiene todas las definiciones de base de datos para la aplicación **Gestor de Pedidos**, incluyendo:

- ✅ Esquema inicial de tablas
- ✅ Datos de precarga
- ✅ Sistema de auditoría
- ✅ Funciones y triggers
- ✅ Gestión de carrito y pagos
- ✅ Gestión de usuarios
- ✅ Reembolsos y devoluciones
- ✅ Metadata de pedidos

## 📚 Requisitos Previos

- **Java 8+** (para ejecutar Liquibase)
- **Maven 3.6+** (recomendado)
- **Base de Datos**: PostgreSQL 12+ (o compatible)
- **Liquibase 4.0+** (incluido en las dependencias del proyecto)

## 📁 Estructura del Proyecto

```
Gestor-de-Pedidos-DB/
├── README.md                          # Este archivo
├── db/
│   ├── changelog/
│   │   ├── db.changelog-master.xml   # Fichero maestro de cambios
│   │   └── changes/
│   │       ├── 001-schema-inicial.xml           # Tablas principales
│   │       ├── 002-inserts-datos.xml            # Datos iniciales
│   │       ├── 003-auditoria-tabla.xml          # Sistema de auditoría
│   │       ├── 004-funciones-triggers.xml       # Funciones y triggers
│   │       ├── 005-carrito-pago.xml             # Carrito y pagos
│   │       ├── 006-usuarios.xml                 # Gestión de usuarios
│   │       ├── 007-fix-enum-columns.xml         # Ajustes de enumeraciones
│   │       ├── 008-pedido-metadata.xml          # Metadata de pedidos
│   │       └── 008-reembolso.xml                # Sistema de reembolsos
│   └── migration/                     # Scripts SQL generados por Liquibase
└── ...
```

## 🚀 Instalación

### 1. Clonar el Repositorio

```bash
git clone <tu-repo-url>
cd Gestor-de-Pedidos-DB
```

### 2. Configurar Base de Datos

Crear base de datos PostgreSQL:

Este proyecto es parte de **Gestor de Pedidos**. Consulta el fichero de licencia en la raíz del proyecto principal.
