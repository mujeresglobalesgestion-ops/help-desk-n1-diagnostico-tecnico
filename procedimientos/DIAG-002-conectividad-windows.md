# DIAG-002 — Conectividad básica en Windows

**Tipo:** procedimiento de laboratorio para formación N1. **Estado:** preparado, pendiente de ejecución en un equipo de práctica.

## Objetivo
Distinguir problemas de conexión local, configuración IP, resolución de nombres y acceso a un servicio.

## Requisitos y seguridad
Usar una red propia o con autorización. No publicar IP privadas, nombres de equipos, usuarios, dominios internos ni datos de clientes.

## Procedimiento
1. Registrar el síntoma: sin conexión Wi-Fi, sin acceso a internet o falla solo una aplicación.
2. Verificar estado del adaptador Wi-Fi/Ethernet y conexión a la red esperada.
3. Abrir **Símbolo del sistema** y ejecutar `ipconfig`; anotar si existe dirección IPv4 y puerta de enlace, sin publicar valores sensibles.
4. Si está autorizado, ejecutar `ping 127.0.0.1` para comprobar la pila local TCP/IP.
5. Comprobar conectividad con un destino permitido por la política del entorno. Un ping fallido no prueba necesariamente caída: ICMP puede estar bloqueado.
6. Usar `nslookup example.com` para observar si hay respuesta DNS; distinguir resolución de nombres de acceso a la web.
7. Registrar resultados y decidir si corresponde derivación a red, equipo o aplicación.

## Plantilla de evidencia
| Prueba | Resultado real | Interpretación |
|---|---|---|
| Adaptador conectado | Pendiente | Pendiente |
| Configuración IP | Pendiente | Pendiente |
| Loopback | Pendiente | Pendiente |
| Destino autorizado | Pendiente | Pendiente |
| DNS | Pendiente | Pendiente |

## Criterios de escalamiento
Escalar ante fallo generalizado, restricciones de red corporativa, necesidad de privilegios, cambios de infraestructura o ausencia de solución autorizada.

## Resultado
**Pendiente de ejecución y validación.** No se inventan comandos ejecutados, mediciones ni una reparación exitosa.
