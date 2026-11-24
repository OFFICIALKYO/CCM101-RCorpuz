# Mission Reflection

Object storage is better suited for storing millions of photos because it stores each file as an independent object with its own metadata and unique ID in a flat structure, instead of fixed blocks tied to one disk. A block storage drive is limited by its size and by the single server it is attached to, so handling millions of images would mean constantly adding disks and managing file systems. Object storage scales out almost without limit and lets files be accessed directly over HTTP through an API.

Docker made deploying MinIO much easier because I did not have to install dependencies or configure the server manually. One `docker run` command downloaded the image, started the container, mapped ports 9000 and 9001, and set the admin credentials through environment variables. The same command works on any machine with Docker, which makes the deployment fast, repeatable, and consistent.

In cloud storage, a bucket is a top-level container that holds objects (files). It is similar to a folder, but it is also the main unit where settings such as access permissions, versioning, and policies are applied. In this lab, I created a bucket named `client-photos` and uploaded a test file to it.

I think large enterprise companies protect their object storage data from server crashes through replication and redundancy. They keep multiple copies of data across different drives, servers, and even data centers or regions, and use techniques like erasure coding to rebuild data if some parts are lost. They also use backups and versioning, so data can be recovered even after hardware failure or accidental deletion.
