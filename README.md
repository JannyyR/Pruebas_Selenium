# 📦 orfeo-ng-qa-automation

> **Skina Technologies** · Suite de pruebas automatizadas, parametrizadas y de regresión funcional para la plataforma Orfeo NG Enterprise utilizando Selenium IDE.

![Selenium](https://img.shields.io/badge/-selenium-%2343B02A?style=for-the-badge\&logo=selenium\&logoColor=white)
![JSON](https://img.shields.io/badge/json-%23000000.svg?style=for-the-badge\&logo=json\&logoColor=white)
![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge\&logo=angular\&logoColor=white)
![PHP](https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge\&logo=php\&logoColor=white)
![Yii2](https://img.shields.io/badge/Yii2-%23E34F26.svg?style=for-the-badge\&logo=yii\&logoColor=white)

---

## 📋 Descripción

**orfeo-ng-qa-automation** es una solución de aseguramiento de calidad (QA) desarrollada durante las prácticas profesionales realizadas en **Skina Technologies S.A.S.**

El proyecto busca reducir los riesgos asociados a regresiones funcionales en **Orfeo NG Enterprise**, una plataforma SGDEA (Sistema de Gestión Documental Electrónico de Archivo), mediante la automatización de pruebas funcionales críticas utilizando Selenium IDE.

La suite permite validar procesos clave relacionados con:

* Autenticación de usuarios.
* Recuperación de contraseñas.
* Visualización de dashboards.
* Gestión documental.
* Navegación por bandejas de radicados.
* Validación de semaforización documental.
* Flujos multiusuario.

🌐 Sitio web: https://skinatech.com

---

## ✨ Funcionalidades automatizadas

### 🔐 Seguridad y autenticación

* Inicio de sesión con diferentes perfiles.
* Validación de credenciales válidas e inválidas.
* Verificación de mensajes de error.
* Recuperación de contraseñas mediante alertas dinámicas.

### 💬 Componentes emergentes

* Validación de ventanas modales y alertas SweetAlert2.
* Verificación de mensajes informativos y de error.

### 📊 Dashboard

* Validación de carga correcta de widgets.
* Verificación de usuarios activos.
* Verificación de usuarios inactivos.
* Consulta de usuarios por dependencia.

### 👥 Flujos multiusuario

* Usuario Funcional (`ufuncional`).
* Jefe de Dependencia (`ujefe`).
* Administrador (`admin`).

### 🧭 Navegación avanzada

* Interacción con componentes Angular.
* Automatización de menús flotantes.
* Navegación por bandejas documentales.

### 🔔 Semaforización documental

* Validación automática de colores de vencimiento.
* Detección de estados mediante propiedades CSS.
* Automatización con ciclos `while` y comandos dinámicos de Selenium IDE.

---

## 🛠️ Stack Tecnológico

| Componente    | Tecnología       | Propósito                 |
| ------------- | ---------------- | ------------------------- |
| Framework QA  | Selenium IDE     | Automatización de pruebas |
| Frontend      | Angular / NodeJS | Interfaz de usuario       |
| Backend       | PHP 8.x + Yii2   | Lógica de negocio         |
| Selectores    | CSS y XPath      | Localización de elementos |
| Formato Suite | JSON (.side)     | Configuración de pruebas  |

---

## 📁 Estructura del Proyecto

```text
orfeo-ng-qa-automation/
│
├── OrfeoNG_Suite.side
│
├── docs/
│   ├── Plan_de_Pruebas.pdf
│   └── Manual_de_Ejecucion.pdf
│
└── database/
    └── credentials_seed.json
```

## ⚙️ Instalación y Ejecución

### Requisitos Previos

* Google Chrome, Microsoft Edge o Mozilla Firefox.
* Extensión Selenium IDE instalada.

### Clonar repositorio

```bash
git clone https://github.com/tu-usuario/orfeo-ng-qa-automation.git

cd orfeo-ng-qa-automation
```

### Abrir proyecto

1. Abrir Selenium IDE.
2. Seleccionar **Open Existing Project**.
3. Cargar:

```text
OrfeoNG_Suite.side
```

### Configurar URL Base

```text
https://orfeong-demo.skinatech.com/
```

### Ejecutar pruebas

* Run Current Test → Ejecutar un caso específico.
* Run All Tests → Ejecutar toda la suite.

---

## 🗺️ Matriz de Casos de Prueba

| ID     | Módulo             | Rol               | Validación            |
| ------ | ------------------ | ----------------- | --------------------- |
| CP1-01 | Login              | Administrador     | Autenticación exitosa |
| CP1-02 | Recuperación Clave | Público           | Alerta SweetAlert2    |
| CP1-04 | Recuperación Clave | Público           | Usuario inexistente   |
| CP1-10 | Login              | Público           | Campos vacíos         |
| CP1-11 | Login              | Público           | Contraseña incorrecta |
| CP2-01 | Dashboard          | Administrador     | Usuarios activos      |
| CP2-05 | Dashboard          | Administrador     | Usuarios inactivos    |
| CP2-13 | Bandeja Radicados  | Usuario Funcional | Menú flotante         |
| CP2-16 | Semaforización     | Usuario Funcional | Validación RGB        |
| CP2-23 | Reportes           | Jefe Dependencia  | Conteo de radicados   |

---

## 📊 Fases del Proyecto

| Fase | Actividad                            | Estado |
| ---- | ------------------------------------ | ------ |
| 1    | Análisis funcional de Orfeo NG       | ✅      |
| 2    | Diseño de casos de prueba            | ✅      |
| 3    | Construcción de scripts Selenium IDE | ✅      |
| 4    | Validación, documentación y entrega  | 🔄     |

---

## 🌍 Impacto en el Área de Soporte

| Dimensión             | Beneficio                           |
| --------------------- | ----------------------------------- |
| 🛡️ Protección de ANS | Reduce riesgos de regresión         |
| ⚡ Eficiencia          | Disminuye tiempos de prueba         |
| 🎯 Precisión          | Verifica reglas críticas de negocio |
| 📈 Escalabilidad      | Facilita mantenimiento futuro       |

---

## 👥 Información del Proyecto

| Campo                   | Detalle                          |
| ----------------------- | -------------------------------- |
| Autora                  | Janny Andreina Rodriguez Requena |
| Programa                | Tecnología en Informática        |
| Universidad             | UNIMINUTO                        |
| Empresa                 | Skina Technologies S.A.S.        |
| Área                    | Soporte Técnico                  |
| Modalidad               | Presencial                       |
| Acompañante Empresarial | Jenny Maritza Gamez Gomez        |
| Docente de Seguimiento  | César Daniel Lavacude Rivera     |

---

## 📄 Licencia

Este proyecto fue desarrollado con fines académicos y de mejora de procesos internos durante la práctica profesional realizada en Skina Technologies S.A.S. Su distribución o comercialización requiere autorización previa de las partes involucradas.
