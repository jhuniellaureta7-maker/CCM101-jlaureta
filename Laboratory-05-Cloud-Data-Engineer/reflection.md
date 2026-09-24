**1. Why is object storage better suited for storing millions of photos compared to a traditional block storage hard drive?**

This laboratory helped me understand why object storage works so well for applications that need to handle millions of photos. Unlike traditional block storage, which is built more for structured, fixed-size data, object storage is designed to handle large volumes of unstructured data like images, videos, and backups. Every file that gets uploaded is stored as its own object, and that's exactly what makes it a good fit for something like a photo-sharing app.

**2. How did using Docker make it easier to deploy the MinIO storage server?**

Docker made deploying MinIO a lot simpler than I expected. I didn't have to manually install or configure each part of the storage server myself  one Docker command handled creating the container, setting up the ports, and applying the login credentials through environment variables. It made the whole process quicker and a lot less messy compared to setting things up manually.

**3. What is a "bucket" in the context of cloud storage?**

A bucket is basically a storage container used to organize and hold objects like images, documents, and other files. For this activity, I created a bucket called `client-photos` and uploaded a sample file into it to test that everything was working.

**4. How do you think large enterprise companies ensure their object storage data is not lost if the physical server crashes?**

I think large companies avoid this problem by keeping multiple copies of their data, running regular backups, and spreading their storage systems across different physical locations. That kind of redundancy means that even if one server goes down, the data is still accessible somewhere else.

**5. How is your confidence in navigating the Linux command line growing?**

My confidence with the Linux command line is definitely growing with each lab. In the previous activity, I picked up the basics of running and managing Docker containers, and this time I got to use those same skills again — deploying MinIO and checking that the container was actually running properly. I also got a clearer picture of how something done entirely through the command line can connect to and power a web-based service. Overall, this lab made me a lot more comfortable working with Docker, Linux commands, and cloud storage concepts in general.
