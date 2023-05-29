# tec-on-premise-deploy
Action de publicación en servidores on-premise, uso de VPN y artefacto de descarga de archivos.



## Uso
 
```yml

- uses: actions/checkout@v3
  with:
    # IP privada VPN asignada a Github
    # Default: ''
    HOST_IP_VPN_WIREGURD_GITHUB: ''

    # Llave privada asignada a la VPN de Github
    # Default: ''
    WIREGUARD_PRIVATE_KEY_GITHUB: ''

    # Llave publica VPN del servidor Endpoint
    # Default: ''
    WIREGUARD_PUBLIC_KEY_ENDPOINT: ''

    # Cadena de IPs permitidas
    # Default: ''
    WIREGUARD_ALLOWED_IPS: ''
    
    # IP publica y puerto para la conexión a la VPN del Endpoint
    # Default: ''
    PUBLIC_IP_AND_PORT_VPN_ENDPOINT: ''
    
    # Puerto SSH
    # Default: ''
    SSH_PORT: ''
        
    # Llave privada del servidor destino
    # Default: ''
    SSH_PRIVATE_KEY: ''
        
    # Nombre del usuario del SSH
    # Default: ''
    SSH_USERNAME: ''

    # IP privada del servidor Endpoint sin mascara
    # Default: ''
    SSH_HOST_IP_VPN_WIREGUARD_ENDPOINT: ''
    
    # IP del servidor destino (PPRD o PROD)
    # Default: ''
    SSH_HOST_IP_DESTINATION_SERVER: ''
    
    # Nombre de usuario del servidor destino (PPRD o PROD)
    # Default: ''
    SSH_USERNAME_DESTINATION_SERVER: ''
 
    # Nombre del proyecto (mismo de la carpeta en el servidor) y directorio de publicado
    # Default: ''
    PROJECT_NAME_IIS: ''
    
    # Ruta del directorio de descarga
    # Default: ''
    PATH_DOWNLOADED: ''
    
    # Copie de forma recursiva directorios de origen completos. Valores válidos: verdadero y falso
    # Default: ''
    RECURSIVELY_COPY: ''
    
    # Habilitar el debug de archivos de descarga y servidor Endpoint
    # Default: 'false'
    # Optional
    DEBUG_FILES: ''

```
