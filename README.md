# AWS-VPC-Lab-Jack
Laboratorio de AWS con VPC, subred pública, subred privada, bastión host y NAT Gateway.
## Objetivo
Construir una arquitectura segura en AWS con VPC, subred pública, subred privada, bastion host y NAT gateway.

## Arquitectura
- VPC: 10.0.0.0/16
- Subred pública: 10.0.1.0/24 -> salida al internet Gateway.
- Subred privada: 10.0.2.0/24 -> Salida al NAT Gateway.
- Bastion Host en la subred  pública.
- Instancia privada en la subred privada.

## Configuración paso a paso
1. Creación de la VPC y subredes.
2. Creación y configuración del Internet Gateway.
3. Creación y configuración de tabla de enrutamiendo para la subred publica y la subred privada
4. Creación del NAT Gateway y asociación a la tabla privada.
5. Lanzaminto de instancias EC2 (bastion y privada).
6. Prueba de conectividad desde la instancia privada (ping a google.com).
7. Eliminación del NAT Gateway para optimizar costo de laboratorio.

## Evidencias
- Consola AWS (VPC).
  ![VPC](VPC.png)
  
- Tabla de Enrutamiento.
  ![Tabla](Tabla.png)

- Instancia EC2
  ![EC2 Instancias](EC2-Instancias.png)

- Diagrama de arquitectura
 ![Arquitectura](Arquitectura.png)

## Conclusiones
Este laboratorio me permitió practicar la creación de una arquitectura segura en AWS, entender cómo funciona el NAT Gateway y cómo optimizar costos eliminando recursos innecesarios. Documentar cada paso me prepara para roles de Cloud Engineer y Security Engineer.
