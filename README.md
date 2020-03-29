# Cluster_User_Activity

Cluster User Activities

data: city_searches.json
Notebook: sessionize_user_activity_travel.ipynb

Data is from a online travel agent site

They store their data in JSON files. Each row in the json shows all different cities which have been searched for by a user within the same session (as well as some other info about the user). That is, if I go to expedia and look for hotels in NY and SF within the same session, the corresponding JSON row will show my user id, some basic info about myself and the two cities.

Travel sites are browsed by two kinds of users. Users who are actually planning a trip and users who just dream about a vacation. The first ones have obviously a much higher purchasing intent.
Users planning a trip often search for cities close to each other, while users who search for cities far away from each other are often just dreaming about a vacation. That is, a user searching for LA, SF and Las Vegas in the same session is much more likely to book a hotel than a user searching for NY, Paris, Kuala Lumpur

In this project, a cluster algorithm was developed,  the user sessions were clustered into two groups: high intent and low intent.
