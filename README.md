# OracleCommerce_RHEL
Oracle Commerce 11.1.0 (Endeca 11.1.0) Docker on RHEL

MDEX 6.5.1 Platform Services 11.1.0 Tools and Framework 11.1.0 CAS 11.1.0


1. Clone the repository.
2. Download packages. File list is given in installables.
3. Unzip the package files and keep the extracted files and directories under installables.
4. To build the image run: docker build -t vz/oc:11.1.0 .
5. After successful build run the container: docker run -d -p 2222:22  -p 8006:8006 -p 8500:8500 -p 8888:8888 -p 15000:15000 -p 15002:15002 -p 15010:15010 --name oc-11.1 vz/oc-11.1.0
6. To login to the container: docker ps --> Copy the container ID and,
docker exec -it <container_ID> bash
