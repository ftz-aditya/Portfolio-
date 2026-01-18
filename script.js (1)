window.onload= function(){
   document.getElementById("html").style.width="90%";
   document.getElementById("css").style.width="80%";
   document.getElementById("js").style.width="70%";
   document.getElementById("python").style.width="60%";
}  
    
   const btn =document.getElementById("btn");
   let mode="light";
   btn.addEventListener("click", () => {
      document.body.classList.toggle("dark");
   if (mode=="light"){mode="dark";
   btn.innerText="LIGHT MODE";
   } else{
      mode="light"; btn.innerText="DARK MODE";
   }
   });
   
   const cards=document.querySelectorAll(".card");
   const popup=document.getElementById("popup");
   const closeBtn=document.getElementById("closeBtn");
   const title=document.getElementById("popupTitle");
   const desc=document.getElementById("popupDesc");
   const tech=document.getElementById("popupTech");
   function openpopup(card){
      title.innerText = card.dataset.title;
      desc.innerText = card.dataset.desc;
      tech.innerText = card.dataset.tech;
      popup.style.display="block";
      
      card.forEach(c => c.classList.remove("active"));
         card.classList.add("active");
      
   } 
   function closepopup(){
      popup.style.display="none";
      card.forEach(c => c.classList.remove("active"));
   } 
   cards.forEach(card =>{
      card.addEventListener("click", ()=> openpopup(card));
   });
   
   closeBtn.addEventListener("click" , closepopup);
   
   popup.addEventListener("click", (e)=> {
      if(e.target ==popup){
         closepopup(); } });
   document.addEventListener("keydown" , (e)=>{
      if(e.key=="Escape"){
         closepopup();
      }
   });
   document.addEventListener("keydown", (e)=>{
      if(e.key=="Escape"){
         popup.style.display="none";
      }
   }
   ); 
   