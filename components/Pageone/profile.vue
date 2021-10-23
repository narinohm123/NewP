<template>
<div>

    <div class="d-flex flex-row">
        <div class="p-2 m-0 w-1/4 h-full w-full h-full  ">
            <div style="display: flex; justify-content: center;">
                <v-sheet class="w-full h-full w-max p-1 d-flex flex-row p-2 " style="display: flex;justify-content: center;" color="white" elevation="2" height="30vh" width="20vw">
                    <div style="display: flex; justify-content: center; width:100%; height:100%;">
                        <img v-for="(profile, index) in profile" :key="index" src="require('${profile.image}')'" width="50%">
                    </div>
                </v-sheet>
            </div>
        </div>

        <!-- <pre>
          {{profile}}
      
        </pre> -->

        <div class="p-0.5 m-1 w-3/4 w-full h-full border-1 line rounded " style="height:76vh; width:75vw; ">

            <div class="d-flex flex-row ">
                <div class="w-max d-flex flex-column items-center " width="30vw">
                    <v-sheet class="w-full h-full w-max p-1 d-flex flex-row p-2 " style="display: flex;justify-content: center;" color="white" elevation="2" height="6vh" width="24vw">
                        <div class="w-max d-flex " width="30vw">
                            <v-card class="p-2 border rounded text-1 bg-yellow-800 w-max " style="background:#F8CBAD; display: flex; justify-content: center;width:10vw; ">ข้อมูลทั่วไป</v-card>
                        </div>
                    </v-sheet>
                    <div class="d-flex flex-row p-1">
                        <v-sheet class="w-full h-full w-max p-1 d-flex flex-row p-2" color="white" elevation="2" height="68.4vh" width="24vw">

                            <div class="w-max p-1 ">
                                <p class="m-0 mb-0 p-1 ">เลขที่ตำแหน่ง</p>
                                <p class="m-0 mb-0 p-1 ">ชื่อ-สกุล(TH)</p>
                                <p class="m-0 mb-0 p-1 ">ชื่อ-สกุล(EN)</p>
                                <p class="m-0 mb-0 p-1 ">ประเภทบุคลากร</p>
                                <p class="m-0 mb-0 p-1 ">สายงาน</p>
                                <p class="m-0 mb-0 p-1 ">ตำแหน่งงาน</p>
                                <p class="m-0 mb-0 p-1 ">ตำแหน่งทางวิชาาการ</p>
                                <p class="m-0 mb-0 p-1 ">ตำแหน่งบริหาร</p>
                                <p class="m-0 mb-0 p-1 ">วันที่เข้าทำงาน</p>
                                <p class="m-0 mb-0 p-1 ">วันที่บรรจุ</p>
                                <p class="m-0 mb-0 p-1 ">สถานะปฏิบัติงาน</p>
                                <p class="m-0 mb-0 p-1 ">วันเดือนปีเกิด</p>
                                <p class="m-0 mb-0 p-1 ">สัญชาติ</p>
                                <p class="m-0 mb-0 p-1 ">ศาสนา</p>
                                <p class="m-0 mb-0 p-1 ">เบอร์โทร</p>
                                <p class="m-0 mb-0 p-1 ">อีเมล ม.พะเยา</p>
                                <p class="m-0 mb-0 p-1 ">อีเมล ส่วนตัว</p>
                                <p class="m-0 mb-0 p-1 ">ที่อยู่ปัจจุบัน</p>
                            </div>
                            <div class="border-l-2 p-1 ">
                                <!-- <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{profile.id_Position}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.name_th}}</p> 
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.name_en}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.personal_type}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.line_of_work}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.position}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.academic_position}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.director_position}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.start_work_date}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.placement_date}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.status_job}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.date_birth}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.nationality}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.religion_con}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.phone}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.email_UP}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.email_private}}</p>
                                <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1 ">{{ profile.address}}</p> -->
                            </div>
                        </v-sheet>
                    </div>
                </div>
                <div class="w-max d-flex flex-column items-center ">
                    <div>
                        <v-sheet class="w-full h-full w-max p-1 d-flex flex-row p-2 " style="display: flex;justify-content: center; " color="white" elevation="2" height="6vh" width="49.5vw">
                            <div class="w-max d-flex " width="30vw">
                                <v-card class="p-2 border rounded text-1 bg-yellow-800 w-max " style="background:#F8CBAD; display: flex; justify-content: center;width:10vw; ">ข้อมูลวุฒิการศึกษา</v-card>
                            </div>
                        </v-sheet>
                    </div>
                    <div class="d-flex flex-row p-1 ">
                        <v-sheet class="w-full h-full w-max p-2 d-flex flex-row " color="white" elevation="2" height="68.4vh" width="49.5vw">
                            <div style="width: 17vw;" >
                                <div class="m-2" >

                                    &ocir; ปริญญาตรี

                                </div>
                                <div class="d-flex flex-row " width="30vw">

                                    <div class="w-max p-1">
                                        <p class="m-0 mb-0 p-1">วุฒิการศึกษา</p>
                                        <p class="m-0 mb-0 p-1">สาขาวิชา</p>
                                        <p class="m-0 mb-0 p-1">สถานศึกษา</p>
                                        <p class="m-0 mb-0 p-1">จังหวัด</p>
                                        <p class="m-0 mb-0 p-1">ประเทศ</p>
                                        <p class="m-0 mb-0 p-1">วันที่เข้าศึกษา</p>
                                        <p class="m-0 mb-0 p-1">วันที่จบการศึกษา</p>
                                        <p class="m-0 mb-0 p-1">เกรดเฉลี่ย</p>
                                        <p class="m-0 mb-0 p-1">เกียรตินิยม</p>
                                        <p class="m-0 mb-0 p-1">วุฒิที่ใช้บรรจุ</p>
                                    </div>
                                    <div class="border-l-2 p-1 ">
                                        <!-- <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.degree}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.faculty}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.university}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.province}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.country}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.study_date}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.graduate}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.gpa}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.honors}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.use_choice_con}}</p> -->
                                    </div>

                                </div>

                            </div>
                            <div style="width: 17vw;" >
                                <div class="m-2">
                                    &ocir; ปริญญาโท
                                </div>
                                <div class="d-flex flex-row ">
                                    <div class="w-max p-1">
                                        <p class="m-0 mb-0 p-1">วุฒิการศึกษา</p>
                                        <p class="m-0 mb-0 p-1">สาขาวิชา</p>
                                        <p class="m-0 mb-0 p-1">สถานศึกษา</p>
                                        <p class="m-0 mb-0 p-1">จังหวัด</p>
                                        <p class="m-0 mb-0 p-1">ประเทศ</p>
                                        <p class="m-0 mb-0 p-1">วันที่เข้าศึกษา</p>
                                        <p class="m-0 mb-0 p-1">วันที่จบการศึกษา</p>
                                        <p class="m-0 mb-0 p-1">เกรดเฉลี่ย</p>
                                        <p class="m-0 mb-0 p-1">เกียรตินิยม</p>
                                        <p class="m-0 mb-0 p-1">วุฒิที่ใช้บรรจุ</p>
                                    </div>
                                    <div class="border-l-2 p-1 ">
                                        <!-- <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.degree_Master}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.faculty_Master}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.university_Master}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.province_Master}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.country_Master}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.study_date_Master}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.graduate_Master}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.gpa_Master}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.honors_Master}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.use_choice_con_Master}}</p> -->
                                    </div>
                                </div>
                            </div>
                            <div>
                                <div class="m-2">
                                    &ocir; ปริญญาเอก
                                </div>
                                <div class="d-flex flex-row ">
                                    <div class="w-max p-1">
                                        <p class="m-0 mb-0 p-1">วุฒิการศึกษา</p>
                                        <p class="m-0 mb-0 p-1">สาขาวิชา</p>
                                        <p class="m-0 mb-0 p-1">สถานศึกษา</p>
                                        <p class="m-0 mb-0 p-1">จังหวัด</p>
                                        <p class="m-0 mb-0 p-1">ประเทศ</p>
                                        <p class="m-0 mb-0 p-1">วันที่เข้าศึกษา</p>
                                        <p class="m-0 mb-0 p-1">วันที่จบการศึกษา</p>
                                        <p class="m-0 mb-0 p-1">เกรดเฉลี่ย</p>
                                        <p class="m-0 mb-0 p-1">เกียรตินิยม</p>
                                        <p class="m-0 mb-0 p-1">วุฒิที่ใช้บรรจุ</p>
                                    </div>
                                    <div class="border-l-2 p-1 ">
                                        <!-- <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.degree_doctorate}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.faculty_doctorate}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.university_doctorate}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.province_doctorate}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.country_doctorate}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.study_date_doctorate}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.graduate_doctorate}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.gpa_doctorate}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.honors_doctorate}}</p>
                                        <p v-for="(profile, index) in profile" :key="index" class="m-0 mb-0 p-1">{{ profile.use_choice_con_doctorate}}</p> -->
                                    </div>
                                </div>
                            </div>
                        </v-sheet>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
import {get , post} from '../../config/service'
import { end_point , api } from '../../config/config';
import axios from '@nuxtjs/axios'
const url  = end_point + api

export default {
//    data() {
//       return {
//         profile: {}
        
//       }
//     },
//     async fetch(){
//         this.form = await fetch(
//             url,
//             console.log(fetch)
//         ).then(res => res.json())
//     },
//     mounted(){
//         this.dataProfile()
//     },
//     methods:{
//         async dataProfile(){
//             let rs = await this.$axios.get('account/user-profile/')
//             console.log(rs)
//         }
//     }
    
}

</script>

<style>
/* .line {
    border: 2px solid black;
    

} */
</style>
