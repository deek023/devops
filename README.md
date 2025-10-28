# devops
Dockerfile:
FROM httpd:latest
COPY hello.html /usr/local/apache2/htdocs

HTML file:
  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Simple Profile Card</title>
  <style>
    /* Basic reset */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background-color: #f0f2f5;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .card {
      background: white;
      width: 320px;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      text-align: center;
    }

    .profile-img {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      margin-bottom: 15px;
      border: 3px solid #4a90e2;
    }
    h2 {
      color: #333;
      margin-bottom: 8px;
    }

    p.title {
      color: #777;
      font-size: 14px;
      margin-bottom: 15px;
    }

    p.description {
      font-size: 15px;
      color: #555;
      margin-bottom: 20px;
    }

    .contact-btn {
      background-color: #4a90e2;
      color: white;
      padding: 10px 25px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      font-weight: bold;
      transition: background-color 0.3s ease;
      text-decoration: none;
      display: inline-block;
    }
    .contact-btn:hover {
      background-color: #357abd;
    }
  </style>
</head>
<body>

  <div class="card">
    <img
      class="profile-img"
      src="https://randomuser.me/api/portraits/women/65.jpg"
      alt="Profile Picture"
    />
    <h2>Jane Doe</h2>
    <p class="title">Front-End Developer</p>
    <p class="description">
      Passionate about crafting beautiful and performant web experiences. Lover of JavaScript and React.
    </p>
    <a href="mailto:jane.doe@example.com" class="contact-btn">Contact</a></div></body>
</html>



B1:
docker build -t <name> .
docker run -d --name <name> -p 8000:80 <name of image>:latest
B2:
After the above:
docker tag <name_image> <username>/<docker_repo_name>:latest
docker push <username>/<docker_repo_name>:latest
docker pull <username>/<docker_repo_name>:latest





advantages of devops:
principles of devops:


A1:
git init
git config --global user.name ""
git config --global user.email ""
git config --global --list
git status
git log
git push --set--upstream 
git reset --soft HEAD~1(gets back to the previous commit)
git reflog
git reset --soft <id>
git config --global --unset user.name 
