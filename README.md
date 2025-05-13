# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>HTML5 Features Example</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
    }
    table {
      border-collapse: collapse;
      width: 100%;
      margin-bottom: 20px;
    }
    th, td {
      border: 1px solid #444;
      padding: 10px;
      text-align: left;
    }
    form {
      max-width: 500px;
      margin-top: 20px;
    }
    label {
      margin-top: 10px;
      display: block;
    }
    input, select, textarea {
      width: 100%;
      padding: 8px;
      margin-top: 4px;
    }
  </style>
</head>
<body>

  <header>
    <h1>Welcome to HTML5 Showcase</h1>
    <p>This page demonstrates HTML5 images, lists, tables, forms, input types, multimedia, and validations.</p>
  </header>

  <!-- HTML5 Image -->
  <section>
    <h2>HTML5 Image</h2>
    <img src="https://images.pexels.com/photos/1103970/pexels-photo-1103970.jpeg" alt="Nature view" width="600"/>
  </section>

  <!-- Ordered and Unordered List -->
  <section>
    <h2>Lists</h2>
    <h3>Ordered List (Roman Numerals)</h3>
    <ol type="I">
      <li>Plan</li>
      <li>Design</li>
      <li>Develop</li>
      <li>Test</li>
      <li>Deploy</li>
    </ol>

    <h3>Unordered List</h3>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
    </ul>
  </section>

  <!-- Contact Table -->
  <section>
    <h2>Contact Table</h2>
    <table>
      <thead>
        <tr>
          <th>Name</th>
          <th>Address</th>
          <th>Mobile</th>
          <th>Email</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Alice Smith</td>
          <td>12 Elm Street, Townsville</td>
          <td>+1234567890</td>
          <td>alice@example.com</td>
        </tr>
        <tr>
          <td>Bob Johnson</td>
          <td>78 Maple Ave, City</td>
          <td>+1987654321</td>
          <td>bob@example.com</td>
        </tr>
        <tr>
          <td>Charlie King</td>
          <td>55 Palm Rd, Capital</td>
          <td>+1223344556</td>
          <td>charlie@example.com</td>
        </tr>
        <tr>
          <td>Diana Hope</td>
          <td>90 Cedar Ln, Suburb</td>
          <td>+1334455667</td>
          <td>diana@example.com</td>
        </tr>
        <tr>
          <td>Edward Lane</td>
          <td>32 Spruce Blvd, Village</td>
          <td>+1445566778</td>
          <td>edward@example.com</td>
        </tr>
      </tbody>
    </table>
  </section>

  <!-- Registration Form -->
  <section>
    <h2>Registration Form</h2>
    <form action="#" method="POST">
      <label for="fullname">Full Name:</label>
      <input type="text" id="fullname" name="fullname" placeholder="Enter your name" required />

      <label for="email">Email:</label>
      <input type="email" id="email" name="email" placeholder="Enter your email" required />

      <label for="password">Password:</label>
      <input type="password" id="password" name="password" placeholder="Enter password" required minlength="6"/>

      <label for="dob">Date of Birth:</label>
      <input type="date" id="dob" name="dob" required />

      <label for="phone">Phone Number:</label>
      <input type="tel" id="phone" name="phone" placeholder="e.g., +1234567890" pattern="^\+\d{10,15}$" required />

      <label for="website">Website:</label>
      <input type="url" id="website" name="website" placeholder="https://example.com"/>

      <label for="country">Country:</label>
      <select id="country" name="country" required>
        <option value="">--Select--</option>
        <option value="us">USA</option>
        <option value="ng">Nigeria</option>
        <option value="uk">UK</option>
      </select>

      <label>Gender:</label>
      <input type="radio" id="male" name="gender" value="male" required />
      <label for="male">Male</label>
      <input type="radio" id="female" name="gender" value="female" />
      <label for="female">Female</label>

      <label>Interests:</label>
      <input type="checkbox" id="coding" name="interests" value="coding" />
      <label for="coding">Coding</label>
      <input type="checkbox" id="music" name="interests" value="music" />
      <label for="music">Music</label>

      <label for="bio">Short Bio:</label>
      <textarea id="bio" name="bio" rows="4" placeholder="Tell us something about you..."></textarea>

      <br/><br/>
      <input type="submit" value="Register"/>
    </form>
  </section>

  <!-- Multimedia Elements -->
  <section>
    <h2>Multimedia</h2>

    <h3>Audio</h3>
    <audio controls>
      <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
      Your browser does not support the audio element.
    </audio>

    <h3>Video</h3>
    <video controls width="600">
      <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
      Your browser does not support the video element.
    </video>
  </section>

  <footer>
    <p>&copy; 2025 HTML5 Practice Page</p>
  </footer>

</body>
</html>
