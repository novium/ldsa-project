# Spark / Hadoop YARN on Docker Swarm

The Hadoop containers are based of off big-data-europe/docker-hadoop with some modifications to support vm/instance-sizes that are appropriate for the allocated usage for the course UPPMAX.

To support other hardware configurations, please edit the `hadoop.env` file. Also, note that the images on Docker Hub might be broken, if you're using this, please build your own images for the nodemanager and the spark/jupyter services.