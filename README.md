# Jupyter notebook playground

--------------------------------------------------------------------------------

### Prerequisites

What things you need to install the software

```
docker 17+
docker-compose 1.19.0+

```

--------------------------------------------------------------------------------

### Installing

```
# Change the directory to the playground folder
cd path-to-your-playground

# Create a .env file with your local playground folder
echo "APP_FOLDER=/path-to-your-playground" > .env

# Build the jupyter notebook environment
sudo docker-compose -f docker/docker-compose.yaml build

```

--------------------------------------------------------------------------------

### Executing

```
# Run the jupyter notebook environment
sudo docker-compose -f docker/docker-compose.yaml up -d

# Execute the jupyter notebook server 
sudo docker exec -it JupiterNotebookPlayground jupyter notebook --notebook-dir=/usr/src/app/notebooks --ip='*' --port=8888 --no-browser --allow-root 

```

--------------------------------------------------------------------------------

## Authors

- **Simone Adelchino** - [github](https://github.com/claclacla)