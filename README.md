<div dir="rtl">
  <h1>الصلاحيات </h1>
 
 
 <p>  هي قيودٌ يفرضها النظام على المستخدمين أثناء استخدامهم للمجلدات والملفات حيث يمكن لبعض المستخدمين التعديل والحذف والبعض القراءه فقط. فهي ترجع لسياسية صاحب النظام.</p>
  <hr>
   <h1>المستخدمين </h1>
  <p>ينقسم المستخدمين في النظام القادرين على التعامل مع الملفات والمجلدات الى ثلاثة أقسام :</p>
   <ul>
  <li>Owner</li>
  <li>Groups</li>
  <li>Other</li>
   </ul>   
 <hr>
  <h1>أنواع الصلاحيات</h1>
     <ul>
  <li>Read</li>
  <li>Write</li>
  <li>Execute</li>
   </ul>   
 <hr>
  <h3> لعرض الصلاحيات </h3>
  <code>ls -l </code>
  <hr>
  <h2>ملاحظة</h2>
  <p> يتم تمثيل المستخدمين والصلاحيات بالحرف الأول </p>
  
   <table>
  <tr>
    <th>Other =>o</th>
    <th>Groups =>g</th>
    <th>Owner =>o</th>
  </tr>
  <tr>
    <td>Execute =>x</td>
    <td>Write =>w</td>
    <td>Read =>r</td>
  </tr>
</table> 
  <hr>
  <h3> للتعديل على الصلاحيات </h3>
  <code> chmode </code>
  <p>اذا كان التعديل يتضمن اضافة صلاحية نستخدم رمز الجمع واذا كان التعديل يتضمن حذف صلاحية نستخدم رمز الطرح </p>
 <p>بعض الامثلة على تعديل الصلاحيات في الملفات او المجلدات</p>
  
    chmod g+w filename
    chmod g-wx filename
    chmod o+w filename
    chmod o-rwx foldername
 <hr>
  <h1>تغير الصلاحيات بالأرقام </h1>
  <p>يمكن تمثيل الصلاحيات بـ استخدام الارقام فـ</p>
       <ul>
  <li>Read => 4 </li>
  <li>Write => 2</li>
  <li>Execute => 1</li>
   </ul>   
   <p> عند اضافة او حذف الصلاحية نضع الرقم الذي يمثل الصلاحية لكن في حال اضافة اكثر من صلاحيه لنفس العنصر فـنقوم بجمع ارقام الصلاحيات الـتي نريدها</p>
  <p> بعض من الامثلة</p>
  <p>
    <code>
    chmod 700 foldername</p>
  chmod 327 foldername 
    </code>
  <hr>
  كل التوفيق .. 
  
 
