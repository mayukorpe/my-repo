
sample_data = {
    "name": "John Doe",
    "age": 30,
    "city": "New York",
    "email": "john@example.com",
    "is_student": False,
    "hobbies": ["reading", "hiking", "photography"],
    "address": {
        "street": "123 Main St",
        "zipcode": "10001"
    }
}

# Convert Python dictionary to JSON string
json_string = json.dumps(sample_data, indent=4)  # Pretty print with indentation
print("JSON String:")
print(json_string)

# Save JSON string to a file
with open('sample_data.json', 'w') as json_file:
    json.dump(sample_data, json_file, indent=4)

# Read JSON data from a file
with open('sample_data.json', 'r') as json_file:
    loaded_data = json.load(json_file)
    print("\nLoaded JSON data:")
    print(loaded_data
