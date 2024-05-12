# Blogging Platform API : 

# Setup and Usage

# Cloning the Repository

git clone https://github.com/ABChaitu79/blogging_platform_api


cd blogging_platform_api

# Installing the dependencies
pip install -r requirements.txt


# Running the API Locally
uvicorn main:app --reload

# API DOCUMENTAION

# CREATING A POST:

Endpoint: POST /posts/
Request Body: JSON object with keys title and content.
Example:
{
    "title": "Sample Title",
    "content": "Sample Content"
}

# READING A POST:

Endpoint: GET /posts/{post_id}
Example: GET /posts/123456

# UPDATING A POST:

Endpoint: PUT /posts/{post_id}
Request Body: JSON object with keys title and content.
Example:
{
    "title": "Updated Title",
    "content": "Updated Content"
}

# DELETING A POST:

Endpoint: DELETE /posts/{post_id}
Example: DELETE /posts/123456

# DATA MODELS

# POST MODEL:
{
    "title": "string",
    "content": "string"
}

# COMMENT MODEL:
{
    "post_id": "string",
    "content": "string"
}

# REACTION MODEL:
{
    "post_id": "string",
    "reaction_type": "string"  # Like or Dislike
}
