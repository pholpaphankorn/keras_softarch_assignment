# keras_softarch_assignment
### TO-DO list:

1. (ยังไม่ได้ทำ)หาและอธิบาย Architectural Styles ของ keras หรือ Architectural Styles ของระบบที่ keras ถูกใช้
	* [ ] วาด UML Diagram(ไม่จำเป็นต้องเป็น class diagram ขอให้เข้าใจง่าย)อย่างน้อย 1 Diagram สำหรับ Architectural Styles ที่หามา
	* [ ] หาข้อเสียอย่างน้อย 1 จุดของ Architectural Stylesและนำเสนอวิธีการแก้ไขข้อเสียตรงนั้น
	
2. (ยังไม่ได้ทำ)หาและอธิบาย quality attributes ของ keras อย่างน้อย 3 ตัวโดยรายละเอียดมีดังนี้:
	* [ ] ให้เหตุผลว่าทำไมคนสร้าง kerasถึงเลือกใช้ quality attributes ตัวนี้
	* [ ] หาและอธิบายว่าคนสร้าง kerasใช้วิธีการอะไรในการทำให้ตอบโจทย์ quality attributes ตัวนั้น
	* [ ] หาหลักฐานมา support ข้อ 1 และ 2(อาจจะเป็น documentationหรือ source code โดยระบุ link และ บรรทัด code) 
	
3. (เจอแล้ว4ตัว)หา design pattern 4 ตัวโดยรายละเอียดมีดังนี้:
	* [ ] อธิบายว่าทำไมแต่ละตัวถึงถูกใช้ใน keras มันเหมาะสมกันยังไง
	* [ ] ระบุ source file และบรรทัด code
	* [ ] (optional-มีไม่มีก็ได้) documentation หรือ commend ของ developer
	* [ ] วาด class diagram สำหรับ design pattern แต่ละตัวที่หามา
	
4. นำเสนอ 15 นาทีเหมือนอาจารย์จะให้พูดทุกคนโดยมีรายละเอียดคร่าวๆดังนี้ - นำเสนอวันที่ 18 หรือ 22 พ.ย. 64
	* [ ] introduction ของ keras ว่าคืออะไรและใช้ทำอะไรคร่าวๆ
	* [ ] อธิบายผลลัพธ์จากการวิเคราะห์ Architectural Stylesของ keras และให้ดู UML diagram
	* [ ] อธิบายผลลัพธ์จากการวิเคราะห์ design pattern ของ keras และให้ดู UML diagram หรือ code บางส่วน

### Design pattern ที่หาเจอและน่าจะถูกต้อง:
	1. Decorator(class Wrappers) - https://github.com/keras-team/keras/blob/3a33d53ea4aca312c5ad650b4883d9bac608a32e/keras/layers/wrappers.py#L34
	2. Iterator(class Iterator) - https://github.com/keras-team/keras/blob/v2.6.0/keras/preprocessing/image.py#L318-L319
	3. Composite(class Sequential) - https://github.com/keras-team/keras/blob/v2.6.0/keras/engine/sequential.py#L41-L467
	4. Adapter(class DataAdapter) - https://github.com/keras-team/keras/blob/3a33d53ea4aca312c5ad650b4883d9bac608a32e/keras/engine/data_adapter.py#L40
