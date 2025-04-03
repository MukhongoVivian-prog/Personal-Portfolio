* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Arial', sans-serif;
}

body {
    background-color: #f4f4f4;
    color: #333;
}

.container {
    width: 90%;
    margin: auto;
    max-width: 1200px;
}

header {
    background: #009688;
    color: white;
    padding: 40px 0;
    text-align: center;
}

header h1 {
    font-size: 3em;
    margin-bottom: 0;
}

header h2 {
    font-size: 1.5em;
}

header .header-text h1 span {
    color: #ff7043;
}

header nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}

header nav ul {
    list-style: none;
    display: flex;
}

header nav ul li {
    margin: 0 15px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    text-transform: uppercase;
    transition: color 0.3s;
}

header nav ul li a:hover {
    color: #ff7043;
}

/* About Section */
#about {
    padding: 60px 0;
    background-color: white;
}

#about h1 {
    text-align: center;
    margin-bottom: 30px;
    color: #333;
}

.about-col-2 {
    width: 50%;
    padding: 20px;
}

.tab-titles {
    display: flex;
    justify-content: space-between;
    margin-top: 20px;
}

.tab-titles p {
    cursor: pointer;
}

.tab-contents {
    display: none;
    margin-top: 20px;
}

.tab-contents.active-tab {
    display: block;
}

/* Projects Section */
#projects {
    padding: 60px 0;
    background-color: #009688;
    color: white;
    text-align: center;
}

.project-list {
    display: flex;
    justify-content: space-between;
    gap: 30px;
    flex-wrap: wrap;
}

.project-list div {
    background-color: #ffffff;
    padding: 30px;
    border-radius: 8px;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
    width: 23%;
    text-align: center;
    transition: all 0.3s ease;
}

.project-list div:hover {
    transform: translateY(-10px);
}

.project-list i {
    font-size: 2.5em;
    margin-bottom: 10px;
}

.project-list h3 {
    margin: 10px 0;
}

.project-list p {
    font-size: 1.1em;
}

.project-list a {
    text-decoration: none;
    color: #ff7043;
    font-weight: bold;
}

/* Contact Section */
#contact {
    background-color: #ffffff;
    padding: 60px 0;
}

#contact .contact-left {
    width: 50%;
    padding: 20px;
    text-align: left;
}

#contact .contact-left h1 {
    font-size: 2em;
}

#contact .contact-left p {
    font-size: 1.1em;
    margin: 15px 0;
}

#contact .contact-right {
    width: 50%;
    padding: 20px;
}

#contact .contact-right form input,
#contact .contact-right form textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 15px;
    border: 1px solid #ddd;
    border-radius: 4px;
}

#contact .contact-right form button {
    padding: 10px 20px;
    background-color: #009688;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

#contact .contact-right form button:hover {
    background-color: #00796b;
}

/* Footer */
footer {
    background-color: #009688;
    color: white;
    padding: 20px 0;
    text-align: center;
}

footer p {
    font-size: 1em;
    margin-top: 10px;
}

.social-icons {
    margin: 20px 0;
}

.social-icons a {
    font-size: 1.5em;
    color: white;
    margin: 0 10px;
    transition: color 0.3s ease;
}

.social-icons a:hover {
    color: #ff7043;
}

@media screen and (max-width: 768px) {
    header nav {
        flex-direction: column;
    }

    .project-list {
        flex-direction: column;
        gap: 20px;
    }

    #about .about-col-2 {
        width: 100%;
    }

    #contact .contact-left,
    #contact .contact-right {
        width: 100%;
    }
}
