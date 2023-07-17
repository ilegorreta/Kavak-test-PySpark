# Kavak-test - Exercise 2 
### Local PySpark dev environment - Based on sample configuration from: jplane/pyspark-devcontainer public GitHub repository

This repository contains the second exercise for the Data Engineering Test.

Here are the exercise instructions:

### Ejercicio 2 (Desarrollar en Spark) [tiempo estimado: 1 hr]
El archivo ```articles.csv``` contiene una tabla con información de artículos que existen en una tienda de
ropa. Deberás:
1. Generar un diccionario a partir de la columna product_type_name
(product_type_no,product_type_name)
2. Escribir el diccionario como CSV
3. Leer el CSV generado y hacer inner join con articles.csv
El dataframe, después del inner join, debe tener el mismo número de registros que el archivo original.
NOTAS:
- No se debe mezclar Pandas con Spark
- No se debe usar koalas para este ejercicio

## Initial Considerations

This repo provides everything needed for a self-contained, local PySpark 1-node "cluster" running on your laptop, including a Jupyter notebook environment.

It uses [Visual Studio Code](https://code.visualstudio.com/) and the [devcontainer feature](https://code.visualstudio.com/docs/devcontainers/containers) to run the Spark/Jupyter server in Docker, connected to a VS Code dev environment frontend.

## Requirements

- Install [Docker Desktop](https://www.docker.com/products/docker-desktop/)

- Install [Visual Studio Code](https://code.visualstudio.com/download)

- Install the [VS Code Remote Development pack](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)

## Setup

1. Install required tools 

2. Git clone this repo to your laptop

3. Open the local repo folder in VS Code

4. Open the [VS Code command palette](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette) and select/type 'Reopen in Container'

5. Wait while the devcontainer is built and initialized, this may take several minutes

6. Open ```src/ejercicio_2.ipynb``` in VS Code

7. If you get an HTTP warning, click 'Yes'

8. Wait a few moments for the Jupyter kernel to initialize... if after about 30 seconds or so the button on the upper-right still says 'Select Kernel', click that and select the option with 'ipykernel'

9. Run the first cell... it will take a few seconds to initialize the kernel and complete. 

10. Run the remaining cells in the notebook!

---
## Directory Tree Structure
It is noteworthy pointing out the directory structure of the repository:

```
├── .devcontainer
│   ├── Dockerfile
│   ├── devcontainer.json
│   └── docker-compose.yaml
├── README.md
├── data
│   ├── articles.csv
│   └── product_type.csv
│       ├── _SUCCESS
│       └── part-00000-1191b6cc-dd3e-498f-b799-2bbadec13086-c000.csv
└── src
    └── ejercicio_2.ipynb
```

## Developed by: Ivan Legorreta
**Phone number**: +52 (55)1320-7574

**Email**: ilegorreta@outlook.com
