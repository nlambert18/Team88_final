# Team88_final
CIT 262 final

How to run:

Open a google Cloud Shell
Clone this repository
Make sure you are in the proper folder thatcontains the YAML file
Run Docker-compose Up

Wait for it to run for a minute or two
Open web preview on port 4567 to open up the STEDI GUi

Use username clinicmanager and password Cl1n1cM@n@ger to log in.
Create new customer.
Enter info on required fields and hit submit.

Run the command and look for the container ids for redis and kafka: docker ps
Look for the customer you created in Redis (you should see JSON with customer data)
From the terminal type: docker exec -it team88_final_redis_1 redis-cli
From the terminal type: keys **
You will see the list of all the Redis tables
Type: zrange Customer 0 -1
