<template>
  <div class="about">
    <h1>This is an about page</h1>
    

Vue อ่านว่า “วิว” เหมือนกับคำว่า view เลย โดยเป็น “progressive framework” สำหรับสร้าง user interface ซึ่ง progressive ก็คือการที่ Vue.js นั้นใช้เป็นเหมือนส่วนเพิ่มความสามารถที่เอาไปใช้งานกับ HTML ซึ่งชื่อ Vue นั้นก็มีที่มาจากการที่ library นี้จะโฟกัสที่การจัดการในส่วนของ view เท่านั้น เพื่อให้สามารถนำ Vue ไปใช้งานร่วมกับ Library อื่นๆได้สะดวก และยังเหมาะกับการทำ Single-Page Applications (SPA) หรือเว็บที่ไม่ต้องเปลี่ยนหน้าบ่อยๆนั่นเอง

ซึ่งข้อดีของ Vue.js คือ จะช่วยให้เราสามารถจัดการกับ element ที่นำมา render บนหน้าเว็บของเราได้ง่ายๆ เช่น 

โดยปกติถ้าเราใช้เพียง JavaScript เวลาต้องการจัดการกับ element ในหน้าเว็บ เราจะต้องเขียน JS ไปแก้ไข DOM โดยตรงเพื่อจัดการกับ element ตาม id หรือ class ก็ว่ากันไป 
แล้วถ้าต้องการแก้ไขกับ element อื่นอีก ก็ต้องเขียน JS ไปแก้ไข DOM เพิ่มอีก 1 บรรทัด
แต่ถ้าเราใช้ Vue เราสามารถใช้สิ่งที่เรียกว่า “component” ซึ่งช่วยให้เราจัดการกับ element ได้โดยไม่ต้องเข้าไปแก้ไข DOM โดยตรง
ทำให้เราจัดการกับ Element ได้ง่ายและช่วยให้อ่านโค้ดได้ง่ายขึ้น ลดขั้นตอนที่ต้องไป get element มาจาก DOM ทุกครั้งที่จะแก้ไข ด้วยการเปลี่ยนค่าใน component แทน
แค่เล่าอย่างเดียวคงไม่เห็นภาพต้องลงมือทำกันซักหน่อย
บทความนี้เป็นเพียงบทความแนะนำเครื่องมือเท่านั้น เลยจะไม่สอนติดตั้งนะ! 

Vue มี sandbox ให้เราได้ไปลองเล่นได้ ซึ่งเวลาลองเล่นถ้าเราลองเปลี่ยนโค้ดแล้วลองเซฟดู ก็จะเห็นผลที่เปลี่ยนแปลงทันที  https://codesandbox.io/s/github/vuejs/vuejs.org/tree/master/src/v2/examples/vue-20-hello-world

***บทความนี้จะใช้ตัวอย่างของ https://vuejs.org/v2/guide/ มาอธิบาย
    
  </div>
</template>
