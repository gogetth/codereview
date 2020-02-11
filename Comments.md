# คอมเมนต์

แพคเกจทุก ๆ แพคเกจควรมีคอมเมนต์ของแพคเกจ มันควรจะอยู่ก่อน ` package ` โดยวางไว้ติด ๆ กันในไฟล์ใดไฟล์หนึ่งในแพคเกจ (มันควรจะปรากฏอยู่ในไฟล์เพียงไฟล์เดียว) คอมเมนต์ของแพคเกจควรจะเริ่มต้นด้วยประโยคที่ขึ้นต้นด้วย "Package _ชื่อแพคเกจ_" และใส่สรุปรายละเอียดการทำงานที่ชัดเจนลงไป รายละเอียดตรงนี้จะถูกนำไปใช้ในลิสต์ของแพคเกจใน godoc

ประโยค และ/หรือ ย่อหน้าถัด ๆ ไป จะบ่งบอกถึงรายละเอียดเพิ่มเติม ประโยคเหล่านั้นควรจะเว้นวรรคให้เหมาะสม

```go
// Package superman implements methods for saving the world.
//
// Experience has shown that a small number of procedures can prove
// helpful when attempting to save the world.
package superman
```

ชนิดของข้อมูล ค่าคงที่ ตัวแปร และฟังก์ชั่นที่อยู่ในระดับสูงสุดควรจะมีคอมเมนต์ โดยที่คอมเมนต์ของ bar ควรจะอยู่ในรูปแบบ "_bar_ floats on high o'er vales and hills." ตัวอักษรตัวแรกของ _bar_ จะต้องไม่เป็นตัวใหญ่ ยกเว้นแต่มันเป็นตัวใหญ่อยู่แล้วในโค้ด

```go
// enterOrbit causes Superman to fly into low Earth orbit, a position
// that presents several possibilities for planet salvation.
func enterOrbit() os.Error {
  ...
}
```

ข้อความที่ถูกย่อหน้าในคอมเมนต์ godoc จะแสดงผลแบบบล็อกที่มีการจัดรูปแบบไว้แล้ว ซึ่งจะช่วยทำให้การใส่ตัวอย่งโค้ดทำได้ง่ายขึ้น

```go
// fight can be used on any enemy and returns whether Superman won.
//
// Examples:
//
//  fight("a random potato")
//  fight(LexLuthor{})
//
func fight(enemy interface{}) bool {
  ...
}
```
