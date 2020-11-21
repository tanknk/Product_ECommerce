# Product_ECommerce

# สำหรับกลุ่ม Shop
## การสร้าง PRODUCT ใหม่
ในการที่จะสร้างสินค้าใหม่ ร้านค้าจำเป็นที่จะต้องกรอกข้อมูลดังนี้ แต่ขออธิบายให้เข้าใจก่อนว่า สินค้า 1 รายการสามารถมีได้หลายหมวดหมู่จึงเก็บเป็น Array และสินค้า 1 รายการมีได้หลายตัวเลือก (นึกถึง Shopee) จึงมีการเก็บ Array ของ Option เอาไว้ด้วย ซึ่งในการที่จะสร้างสินค้าใหม่ ร้านค้าจำเป็นที่จะต้องกรอกอย่างน้อย 1 ตัวเลือก หากต้องการเพิ่มตัวเลือกใหม่จะมี api สำหรับเพิ่มตัวเลือกอีกที ซึ่งต้องกรอกข้อมูลดังนี้สำหรับการสร้างสินค้า
* ชื่อหลักของสินค้า (nameMain) : String
* รูปภาพหลักของสินค้า (pictureMain) : String (URL ของรูปภาพ)
* รายละเอียดของสินค้า (description) : String
* อะเรย์ของ Category Id (categorysId) : Array<Int>
* ชื่อของตัวเลือก (nameOption) : String
* ราคาของตัวเลือก (price) : double
* จำนวนสินค้าของตัวเลือก (amount) : int
* รูปภาพของตัวเลือก (pictureOption) : String (URL ของรูปภาพ)
* น้ำหนักของตัวเลือก (weight) : double
* รหัสของร้านค้าที่สร้างสินค้า (shop_id) : int
  
![](https://github.com/tanknk/Product_ECommerce/blob/main/images/create1.png)
![](https://github.com/tanknk/Product_ECommerce/blob/main/images/create2.png)

## การสร้าง OPTION ใหม่
ในการสร้างตัวเลือกของสินค้าใหม่ ร้านค้าจำเป็นที่จะต้องกรอกข้อมูลดังนี้ โดยหลังจากกรอกข้อมูลครบถ้วน จะทำการสร้างตัวเลือกใหม่ภายใน productId ที่กำหนดไว้
* รหัสของสินค้า (productId) : int
* ชื่อของตัวเลือก (name) : String
* ราคาของตัวเลือก (price) : double
* จำนวนสินค้าของตัวเลือก (amount) : int
* รูปภาพของตัวเลือก (picture) : String (URL ของรูปภาพ)
* น้ำหนักของตัวเลือก (weight) : double

![](https://github.com/tanknk/Product_ECommerce/blob/main/images/option1.png)
![](https://github.com/tanknk/Product_ECommerce/blob/main/images/option2.png)

## การดึงข้อมูลของสินค้าด้วย shop_id
ในการที่จะดึงข้อมูลของสินค้าด้วย shop_id สามารถทำได้โดยการกรอก shop_id ดังนี้ โดยผู้ใช้จะได้รับเป็นอะเรย์ของสินค้าที่ shop ที่มี id ตรงกับที่กรอกเข้ามา
![](https://github.com/tanknk/Product_ECommerce/blob/main/images/shop1.png)
![](https://github.com/tanknk/Product_ECommerce/blob/main/images/shop2.png)
![](https://github.com/tanknk/Product_ECommerce/blob/main/images/shop3.png)
