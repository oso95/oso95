<!DOCTYPE html>
<html>
<head>

<style>
 #typing-text {
     color: #66FF00;
     border: solid 1px #A8A8A8;
     font-weight: bold;
     text-align: center;
     font-family: Arial, Helvetica, sans-serif;
     overflow: auto;
     background-color: #000000;
     font-size: 15px;
     padding: 1px;
     height: 250px;
     width: 350px;
     outline: none;
     resize: none;
     box-sizing: border-box;
}

</style>
</head>
<body>
<textarea id="typing-text" readonly></textarea>


<script>
(function () {
   var CharacterPos = 0;
   var MsgBuffer = "";
   var TypeDelay = 80; 
   var NxtMsgDelay = 1000;
   var MsgIndex = 0;
   var delay;
   var MsgArray = ["\n\n\n\n\n\n\nHi, Welcome to my Github page....","\n\n\n\n\n\n\nI am Cheng-Yuan Wang"];

   function StartTyping() {
      var id = document.getElementById("typing-text");
      if (CharacterPos != MsgArray[MsgIndex].length) {
         MsgBuffer  = MsgBuffer + MsgArray[MsgIndex].charAt(CharacterPos);
         id.value = MsgBuffer+"_";
         delay = TypeDelay;
         id.scrollTop = id.scrollHeight; 
      } else {
         delay = NxtMsgDelay;
         MsgBuffer   = "";
         CharacterPos = -1;
         if (MsgIndex!=MsgArray.length-1){
           MsgIndex++;
         }else {
           MsgIndex = 0;
         }
       }
       CharacterPos++;
       setTimeout(StartTyping,delay);
   }
StartTyping();
})();
</script>

</body>
</html>


- 👋 Hi, I’m @cywang95
- 👀 I’m interested in programming
- 🌱 I’m currently learning Swift
- 💞️ I’m looking to collaborate on anything that can give me improvment 
- 📫 How to reach me cyw@cywang.me


<Everytime I Compile the code, I feel like I am creating a world> - cywang

[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=cywang95&theme=dark)](https://git.io/streak-stats)![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=cywang95&count_private=true&show_icons=true&theme=tokyonight)

<!---
cywang95/cywang95 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
