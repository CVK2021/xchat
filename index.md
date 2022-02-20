
<body class="home page-template page-template-front-page page-template-front-page-php page">
<div class="ready" id="webchat-app-bot">
<script>
(function (window, document) {
var createBot = function () {
var params = {
};
BotChat.Intro({ onRequestLive: function () { window.location = "mailto:st@sadalestikls.lv" } }, document.getElementById("webchat-app-bot"));
};
var loadChat = function () {
var script = document.createElement("script"),
link = document.createElement("link");
script.src = "https://st-va.azurewebsites.net/botchat.min.js";
link.href = "https://st-va.azurewebsites.net/botchat.min.css";
link.rel = "stylesheet";
script.onload = createBot;
script.charset = "utf-8";
document.head.appendChild(link);
document.head.appendChild(script);
};
window.addEventListener ? window.addEventListener("load", loadChat, false) : window.attachEvent("onload", loadChat);
})(window, document);
  window.onload=function(){
  document.getElementById("webchat-app-bot").click();
};
</script>
</div>
</body>
