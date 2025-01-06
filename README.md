let liked = false;

function toggleLike() {
    const likeBtn = document.getElementById("like-btn");
    liked = !liked;
    
    if (liked) {
        likeBtn.classList.add("liked");
        document.getElementById("like-count").textContent = parseInt(document.getElementById("like-count").textContent) + 1;
    } else {
        likeBtn.classList.remove("liked");
        document.getElementById("like-count").textContent = parseInt(document.getElementById("like-count").textContent) - 1;
    }
}

function showComments() {
    const commentSection = document.getElementById("comment-section");
    commentSection.style.display = commentSection.style.display === 'none' ? 'block' : 'none';
}

function postComment() {
    const commentInput = document.getElementById("comment-input");
    const commentList = document.getElementById("comment-list");

    if (commentInput.value.trim() !== "") {
        const comment = document.createElement("div");
        comment.classList.add("comment");
        comment.textContent = commentInput.value;
        commentList.appendChild(comment);
        commentInput.value = "";
    }
}body, html {
    margin: 0;
    padding: 0;
    height: 100%;
    font-family: Arial, sans-serif;
    background-color: #000;
}

.app {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.video-container {
    position: relative;
}

.video {
    width: 100%;
    height: auto;
    max-width: 500px;
}

.overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    color: white;
    padding: 20px;
}

.likes, .comments {
    display: flex;
    justify-content: space-between;
}

#like-btn {
    background-color: transparent;
    border: none;
    color: white;
    font-size: 30px;
    cursor: pointer;
}

#like-btn.liked {
    color: red;
}

.comment-section {
    padding: 20px;
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
    background-color: white;
}

#comment-input {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #ddd;
}

button {
    padding: 10px;
    background-color: #ff0000;
    color: white;
    border: none;
    cursor: pointer;
}

button:hover {
    background-color: #cc0000;
}

#comment-list {
    margin-top: 10px;
}

.comment {
    background-color: #f9f9f9;
    padding: 5px;
    margin: 5px 0;
    border-radius: 3px;
}body, html {
    margin: 0;
    padding: 0;
    height: 100%;
    font-family: Arial, sans-serif;
    background-color: #000;
}

.app {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.video-container {
    position: relative;
}

.video {
    width: 100%;
    height: auto;
    max-width: 500px;
}

.overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    color: white;
    padding: 20px;
}

.likes, .comments {
    display: flex;
    justify-content: space-between;
}

#like-btn {
    background-color: transparent;
    border: none;
    color: white;
    font-size: 30px;
    cursor: pointer;
}

#like-btn.liked {
    color: red;
}

.comment-section {
    padding: 20px;
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
    background-color: white;
}

#comment-input {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #ddd;
}

button {
    padding: 10px;
    background-color: #ff0000;
    color: white;
    border: none;
    cursor: pointer;
}

button:hover {
    background-color: #cc0000;
}

#comment-list {
    margin-top: 10px;
}

.comment {
    background-color: #f9f9f9;
    padding: 5px;
    margin: 5px 0;
    border-radius: 3px;
}body, html {
    margin: 0;
    padding: 0;
    height: 100%;
    font-family: Arial, sans-serif;
    background-color: #000;
}

.app {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.video-container {
    position: relative;
}

.video {
    width: 100%;
    height: auto;
    max-width: 500px;
}

.overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    color: white;
    padding: 20px;
}

.likes, .comments {
    display: flex;
    justify-content: space-between;
}

#like-btn {
    background-color: transparent;
    border: none;
    color: white;
    font-size: 30px;
    cursor: pointer;
}

#like-btn.liked {
    color: red;
}

.comment-section {
    padding: 20px;
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
    background-color: white;
}

#comment-input {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #ddd;
}

button {
    padding: 10px;
    background-color: #ff0000;
    color: white;
    border: none;
    cursor: pointer;
}

button:hover {
    background-color: #cc0000;
}

#comment-list {
    margin-top: 10px;
}

.comment {
    background-color: #f9f9f9;body, html {
    margin: 0;
    padding: 0;
    height: 100%;
    font-family: Arial, sans-serif;
    background-color: #000;
}

.app {
    display: flex;
    justify-content: center;let liked = false;

function toggleLike() {
    const likeBtn = document.getElementById("like-btn");
    liked = !liked;
    
    if (liked) {
        likeBtn.classList.add("liked");
        document.getElementById("like-count").textContent = parseInt(document.getElementById("like-count").textContent) + 1;
    } else {
        likeBtn.classList.remove("liked");
        document.getElementById("like-count").textContent = parseInt(document.getElementById("like-count").textContent) - 1;
    }
}

function showComments() {
    const commentSection = document.getElementById("comment-section");
    commentSection.style.display = commentSection.style.display === 'none' ? 'block' : 'none';
}

function postComment() {
    const commentInput = document.getElementById("comment-input");
    const commentList = document.getElementById("comment-list");

    if (commentInput.value.trim() !== "") {
        const comment = document.createElement("div");
        comment.classList.add("comment");
        comment.textContent = commentInput.value;
        commentList.appendChild(comment);
        commentInput.value = "";
    }
}
    align-items: center;
    height: 100vh;
}

.video-container {
    position: relative;
}

.video {
    width: 100%;
    height: auto;
    max-width: 500px;
}

.overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    color: white;
    padding: 20px;
}

.likes, .comments {
    display: flex;
    justify-content: space-between;
}

#like-btn {
    background-color: transparent;
    border: none;
    color: white;
    font-size: 30px;
    cursor: pointer;
}

#like-btn.liked {
    color: red;
}

.comment-section {
    padding: 20px;
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
    background-color: white;
}

#comment-input {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #ddd;
}

button {
    padding: 10px;
    background-color: #ff0000;
    color: white;
    border: none;
    cursor: pointer;
}

button:hover {
    background-color: #cc0000;
}

#comment-list {
    margin-top: 10px;
}

.comment {
    background-color: #f9f9f9;
    padding: 5px;
    margin: 5px 0;
    border-radius: 3px;
}
    padding: 5px;
    margin: 5px 0;
    border-radius: 3px;
}
