# Devops-three-tier-project-deployment-on-AWS
Your Ultimate Travel Blog

1.Start Your Open Source Journey: It's aimed to kickstart your open-source journey. Here, you'll learn the basics of Git and get a solid grip on the MERN stack and I strongly believe that learning and building should go hand in hand.

2.React Mastery: Once you've got the basics down, a whole new adventure begins of mastering React. This project covers everything, from simple form validation to advanced performance enhancements. And I've planned much more cool stuff to add in the near future if the project hits more number of contributors.

Setting up the project locally
Setting up the Backend
Fork and Clone the Repository

git clone https://github.com/{your-username}/wanderlust.git
Navigate to the Backend Directory

cd backend
Install Required Dependencies

npm i
Set up your MongoDB Database

Open MongoDB Compass and connect MongoDB locally at mongodb://localhost:27017.
Import sample data

To populate the database with sample posts, you can copy the content from the backend/data/sample_posts.json file and insert it as a document in the wanderlust/posts collection in your local MongoDB database using either MongoDB Compass or mongoimport.

mongoimport --db wanderlust --collection posts --file ./data/sample_posts.json --jsonArray
Configure Environment Variables

cp .env.sample .env
Start the Backend Server

npm start
You should see the following on your terminal output on successful setup.

[BACKEND] Server is running on port 5000
[BACKEND] Database connected: mongodb://127.0.0.1/wanderlust
Setting up the Frontend
Open a New Terminal

cd frontend
Install Dependencies

npm i


Configure Environment Variables

cp .env.sample .env.local
Launch the Development Server

npm run dev
