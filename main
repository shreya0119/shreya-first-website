const myImage = document.querySelector("img");

myImage.addEventListener("click", () => {
  const mySrc = myImage.getAttribute("src");
  if (mySrc === "images/Kedarji.jpg") {
    myImage.setAttribute("src", "images/Himalyas.jpg");
  } else {
    myImage.setAttribute("src", "images/Kedarji.jpg");
  }
});
let myButton = document.querySelector("button");
let myHeading = document.querySelector("h1");
function setUserName() {
  const myName = prompt("Please enter your name.");
  if (!myName) {
    setUserName();
  } else {
    localStorage.setItem("name", myName);
    myHeading.textContent = `Bholenath ki krupa aap par bani rahe ${myName}`;
  }
}
if (!localStorage.getItem("name")) {
  setUserName();
} else {
  const storedName = localStorage.getItem("name");
  myHeading.textContent = `Bholenath ki krupa aap par bani rahe, ${storedName}`;
}
myButton.addEventListener("click", () => {
  setUserName();
});
