<template>
  <div class="d-flex mb-6 ">
    <div class="d-flex justify-content: flex-start;">
      <img src="@/assets/New.PNG" alt="" width="90%">
    </div>

    <div class="d-block widtter">
      <div class="d-flex justify-end">
        <div class="d-flex align-center mr-5 ">
          <p style="margin-right: 17rem; margin-top: 1.50rem;">ผู้ใช้งาน : </p>
        </div>
        <div>
          <v-btn large x-large x-small style="margin-top: 0.50rem;">ออกจากระบบ</v-btn>
        </div>
      </div>


        <div class="Hd" style="display: flex; width: 100%; height: 53%; justify-content: flex-end; align-items: center;">
      <div class="Box" style="display: flex; width: 95%;">
        <v-app-bar
          class="display: flex; justify-content: space-between"
          color="#AE78D6"
          dense
          dark
        >
          <div class="text-center ">
            <v-menu offset-y>
              <template v-slot:activator="{ on, attrs }">
                <v-btn color="#AE78D6" dark v-bind="attrs" v-on="on" style="width: 165%;">
                  ข้อมูลบุคลากร
                </v-btn>
              </template>
              <v-list>
                <v-list-item v-for="(information, index) in information" :key="index" @click="ContactTabinformation = index" :class="{active: ContactTab === index}">
                  <v-list-item-title>{{ information }}</v-list-item-title>
                </v-list-item>
              </v-list>
            </v-menu>
          </div>

          <div class="text-center">
            <v-menu offset-y>
              <template v-slot:activator="{ on, attrs }">
                <v-btn color="#AE78D6" dark v-bind="attrs" v-on="on" style="width: 150%;">
                  การพัฒนาตนเอง
                </v-btn>
              </template>
              <v-list>
                <v-list-item v-for="(development, index) in development" :key="index" @click="ContactTabdevelopment = index" :class="{active: ContactTab === index}">
                  <v-list-item-title>{{ development }}</v-list-item-title>
                </v-list-item>
              </v-list>
            </v-menu>
          </div>

          <div class="text-center">
            <v-menu offset-y>
              <template v-slot:activator="{ on, attrs }">
                <v-btn color="#AE78D6" dark v-bind="attrs" v-on="on" style="width: 140%;">
                  ตำแหน่งทางวิชาการ
                </v-btn>
              </template>
              <v-list>
                <v-list-item v-for="(position, index) in position" :key="index" @click="ContactTabposition = index" :class="{active: ContactTab === index}">
                  <v-list-item-title>{{ position }}</v-list-item-title>
                </v-list-item>
              </v-list>
            </v-menu>
          </div>

          <div class="text-center">
            <v-menu offset-y>
              <template v-slot:activator="{ on, attrs }">
                <v-btn color="#AE78D6" dark v-bind="attrs" v-on="on" style="width: 140%;">
                  แผนพัฒนาบุคลากร
                </v-btn>
              </template>
            </v-menu>
          </div>

          <div class="text-center">
            <v-menu offset-y>
              <template v-slot:activator="{ on, attrs }">
                <v-btn color="#AE78D6" dark v-bind="attrs" v-on="on" @click="login">
                  รายงานผลการดำเนินงาน
                </v-btn>
              </template>
            </v-menu>
          </div>
        </v-app-bar> 
    </div>
  </div> 
      <div class="Homepage">
          <v-btn depressed outlined plain raised >หน้าเเรก</v-btn>
      </div>
    </div>
  </div>
  
</template>

<script>
export default {
  data: () => {
    return ({
      ContactTabinformation: 0,
      information: ['ข้อมูลส่วนตัว','ข้อมูลบุคลากร' ,'ข้อมูลอัตรากำลัง' ],

      ContactTabdevelopment: 0,
      development: ['ข้อมูลการอบรม/สัมมนา/ดูงาน' ,'ข้อมูลการใช้งบประมาณพัฒนาศักยภาพ' ,'ข้อมูลการลาศึกษา','ข้อมูลบุคลากรดีเด่น'],

      ContactTabposition: 0,
      position: ['สถานะดำเนินการ','เอกสารประกอบการสอน / คำสอน' ,'ผู้ดำรงตำแหน่งทางวิชาการ' ]
    })
  }
};
</script>

<style>
.test{
  border: 1px solid black;
}
.widtter{
  width: 100%;
}
.higther{
  height: 100%;
  /* height: auto; */
}
/* .Hd {
  position: relative;
  top: -120px;
  left: -20px;
} */
/* .Img {
  width: 23%;
  position: relative;
  top: -50px;
  left: 5px;
} */

.Box {
  width: 70%;
  display: flex;
}
.v-toolbar__content,
.v-toolbar__extension {
  align-items: center;
  display: flex;
  justify-content: space-between;
  
}
.Homepage{
  position: relative;
  left: -1rem;
}
</style>

