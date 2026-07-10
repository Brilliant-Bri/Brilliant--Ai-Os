# Brilliant--Ai-Os
Add a README file
Add Brilliant AI OS dashboard core
const BrilliantMemory = {
 save(key,value){
   localStorage.setItem(key, JSON.stringify(value));
 },

 load(key){
   return JSON.parse(localStorage.getItem(key));
 }
}

