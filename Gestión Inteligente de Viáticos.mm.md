# Mapa de Navegación del Sistema - ViaTech

## Vistas principales del sistema

1. **Inicio de Sesión (Login)**
   - URL: `/login`
   - Descripción: Permite la autenticación de los usuarios con credenciales.

2. **Registro de Usuarios**
   - URL: `/register`
   - Descripción: Proceso para registrar nuevos usuarios en el sistema.

3. **Página Principal**
   - URL: `/home`
   - Descripción: Acceso a las funcionalidades principales del sistema.
   - Subvistas:
     - **Gestión de usuarios (Administrador)**
       - URL: `/admin/users`
       - Descripción: Crear, editar y eliminar usuarios, asignar roles y permisos.
     - **Solicitudes (Coordinador)**
       - URL: `/coordinator/requests`
       - Descripción: Revisar y aprobar solicitudes de viáticos, generar reportes de solicitudes.
     - **Actividades y reportes (Director)**
       - URL: `/director/reports`
       - Descripción: Monitorear actividades, generar reportes de desempeño.
     - **Desembolsos (Nómina)**
       - URL: `/payroll/disbursements`
       - Descripción: Procesar pagos de viáticos, generar comprobantes de pago.
     - **Generación de informes**
       - URL: `/reports/generate`
       - Descripción: Crear informes detallados sobre las actividades y desembolsos.

4. **Pantalla de error**
   - URL: `/error`
   - Descripción: Mensajes de error y soluciones comunes.

---

## Flujo de navegación

### Usuario General
1. **Acceso Inicial:**
   - `/login` → `/register` (si no tiene cuenta).
2. **Acceso exitoso:**
   - Redirige a la página asignada según el rol del usuario:
     - Administrador: `/admin`
     - Coordinador: `/coordinator`
     - Director: `/director`
     - Nómina: `/nomina`

---

Este mapa organiza el flujo de navegación dentro del sistema **ViaTech**, asegurando que cada rol acceda únicamente a las funcionalidades específicas de su perfil.
