
# RiseTalk NFT

## Descripción

RiseTalk NFT es un contrato inteligente desarrollado en Clarity para la red Stacks. Este proyecto implementa la funcionalidad para acuñar y transferir NFTs que servirán como certificados digitales para el proyecto RiseTalk, proporcionando una mayor veracidad y autenticidad a los certificados emitidos.

## Características

- Acuñación de NFTs como certificados digitales
- Transferencia de NFTs entre usuarios
- Almacenamiento de metadatos en IPFS
- Implementación del estándar NFT de Stacks

## Estructura del Proyecto

El proyecto está estructurado de la siguiente manera:

- `contracts/risetalk-nft.clar`: Contrato principal de NFT
- `Clarinet.toml`: Configuración del proyecto Clarinet
- `package.json`: Dependencias y scripts del proyecto
- `tsconfig.json`: Configuración de TypeScript
- `vitest.config.js`: Configuración de Vitest para pruebas

## Requisitos

- Node.js
- Clarinet
- Stacks CLI


```

## Uso

## Commands

### Check it is all correct
```
clarinet check
```

### Run contract in devnet
```
clarinet console
```

### Generate deployment plan
```
clarinet deployment generate --testnet --low-cost
```

### Complete deployment
```
clarinet deployment apply -p deployments/default.testnet-plan.yaml

## Funciones Principales

El contrato `risetalk-nft.clar` incluye las siguientes funciones principales:

- `mint`: Acuña un nuevo NFT
- `transfer`: Transfiere un NFT entre usuarios
- `get-last-token-id`: Obtiene el ID del último token acuñado
- `get-owner`: Obtiene el propietario de un token específico
- `get-token-uri`: Obtiene el URI (IPFS hash) de un token específico

## Desarrollo

El proyecto utiliza Clarinet para el desarrollo y pruebas locales. Asegúrate de tener Clarinet instalado y configurado correctamente.

## Licencia

Este proyecto está licenciado bajo ISC, como se especifica en el archivo `package.json`.