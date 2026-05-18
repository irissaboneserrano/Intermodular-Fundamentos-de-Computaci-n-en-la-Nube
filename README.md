# Intermodular-Fundamentos-de-Computaci-n-en-la-Nube
# Proyecto Intermodular
## Fundamentos de Computación en la Nube
### 1º SMR

**Alumno:** Iris Saboné Serrano

---

## 1. Elección de proveedor Cloud

He elegido **Amazon Web Service (AWS)** como proveedor de servicios en la nube.

Se ha elegido porque AWS es una de las plataformas más **utilizadas** a nivel mundial, ofreciendo una gran variedad de **servicios**, alta **disponibilidad** y **escalabilidad**.

AWS es adecuado porque permite **almacenar archivos** de forma segura, crear **servidores** virtuales y **gestionar** sin necesidad de invertir en una **infraestructura física**.

Entre sus principales ventajas destacan la **escalabilidad**, permitiendo ampliar recursos según necesidades, también alta **disponibilidad** y **fiabilidad**, **seguridad** en el acceso de datos y **pago** por uso, evitando grandes inversiones iniciales.

---

## 2. Arquitectura cloud propuesta

La arquitectura propuesta se basa en el uso de servicios en la nube para gestionar el almacenamiento de datos y el acceso a aplicaciones.

La aplicación se ejecutaría en un **servidor virtual** en la nube mediante **EC2**.

Los **datos** de la empresa, como archivos de diseño o documentos, se almacenarían en **Amazon S3.**

En caso de necesitar una **base de datos**, se podría utilizar **Amazon RDS.**

Los usuarios accederían a los recursos a través de **Internet** desde sus equipos, utilizando credenciales gestionadas mediante **AWS IAM**, lo que permite controlar los permisos de acceso.

**Esquema de arquitectura:**

```
Usuarios / Administrador
        ↓
    Internet
        ↓
  Internet Gateway
        ↓
  Amazon EC2 (servidor web / aplicación)  [Public subnet]
     ↙              ↘
Amazon S3         Amazon RDS       [Private subnet]
(almacenamiento    (base de datos)
 de archivos)

AWS IAM → Gestión de usuarios y permisos
```

---

## 3. Servicios cloud utilizados

Para la ejecución del sistema en la nube se utilizarán los siguientes servicios:

- **Amazon S3:** almacenamiento de archivos de la empresa.
- **Amazon EC2:** realización de aplicaciones o servicios necesarios.
- **AWS IAM:** gestión de usuarios y permisos de acceso.
- **Amazon RDS:** gestión de bases de datos en caso de ser necesario.

---

## 4. Estimación de costes

El coste de los servicios en la nube dependerá del uso de los recursos. **AWS ofrece un nivel gratuito (Free Tier)** que permite utilizar algunos servicios con limitaciones durante un periodo inicial.

Por ejemplo:

- Uso limitado de almacenamiento en S3
- Horas gratuitas en servidores EC2
- Acceso básico a otros servicios

Para una pequeña empresa, el coste estimado puede rondar entre los **20 y 50 euros mensuales**, dependiendo del **uso** de almacenamiento, servidores y servicios adicionales.

El uso del **nivel gratuito** permite reducir costes en las primeras fases del proyecto.
