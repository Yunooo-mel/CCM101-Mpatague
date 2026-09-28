# Mission Reflection

**1. Why is object storage better suited for millions of photos than a block storage hard drive?**
Block storage behaves like a single disk attached to one server, so it has fixed capacity and needs manual resizing. Object storage keeps each photo as an independent object in a flat structure, so it can scale to millions of files without folder limits. Each object carries metadata and is reachable through a simple web API, which suits a photo-sharing app. It is also cheaper per gigabyte for large, rarely changed files.

**2. How did Docker make deploying MinIO easier?**
Docker let me deploy MinIO with one command. I did not have to install dependencies or configure the server by hand, because the image already had everything needed. Port mapping and environment variables let me set the ports and login credentials right in the command. If something broke, I could remove the container and start a fresh one in seconds.

**3. What is a bucket?**
A bucket is a top-level container in object storage that holds objects (files). It works like a named storage space, and access rules and settings can be applied to it. In this lab, `client-photos` was the bucket that held the uploaded test file.

**4. How do enterprises keep object storage data safe if a server crashes?**
They use replication, keeping several copies of each object on different drives, servers, and even data centers. Techniques like erasure coding split data into pieces so it can be rebuilt if some pieces are lost. Regular backups and monitoring add another layer of protection, so one failed machine does not cause data loss.

**5. How is my confidence with the Linux command line growing?**
I am more comfortable typing commands like `docker run` and `docker ps` and understanding what each flag does. At first long commands felt intimidating, but breaking them into parts made them easier to read. I still want to practice more, but I now feel I can deploy and verify a service from the terminal on my own.
