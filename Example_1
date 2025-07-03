from pymongo import MongoClient

# Connect to the MongoDB server running on localhost
client = MongoClient('localhost', 27017)

# Access a specific database
db = client['my_database']

# Access a specific collection within the database
users_collection = db['users']

# Insert a new document into the collection
user = {
    'name': 'Sapna Baranwal',
    'age': 23,
    'email': 'sapna.barnwal20010@gmail.com'
}
result = users_collection.insert_one(user)
print("User inserted successfully:", result.inserted_id)

# Find all users in the collection
all_users = users_collection.find()
print("All users:")
for user in all_users:
    print(user)

# Close the connection to the MongoDB server
client.close()
