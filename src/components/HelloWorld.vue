<template>
  <v-container fluid grid-list-lg>
    <v-layout text-center wrap >
      <v-carousel
    cycle
    height="450"
    hide-delimiter-background
    show-arrows-on-hover
  >
  
      <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    >
     </v-carousel-item>
 
  </v-carousel>
   
       <v-flex mb-4 style="background-color:gray"><v-img src="../assets/5.jpg">  
        <h2 class="display-2 font-weight-bold mb-1" >智慧医院信息平台</h2>
        <p class="subheading font-weight-regular">以电子病历为核心的智慧医院信息平台</p>
      </v-img>
      </v-flex>
   
      <v-flex mb-5 xs4 ><v-img src="../assets/8.jpg"> 
        <h1 class="headline font-weight-bold mb-3" >医疗管理系统</h1>

        <v-layout justify-center wrap>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title>
                <a
                  v-for="(next, i) in healthCare"
                  :key="i"
                  :href="next.href"
                  class="subheading mx-3"
                  target="_blank" 
                  style="color:burlywood"
                >{{ next.text }}<br></a>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-layout>
      </v-img>
      </v-flex>

      <v-flex xs4 mb-5 ><v-img src="../assets/6.jpg"> 
        <h2 class="headline font-weight-bold mb-3">临床服务系统</h2>

        <v-layout justify-center row wrap>
          <v-flex d-flex>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title>
                <a
                  v-for="(link, i) in clinicSrv"
                  :key="i"
                  :href="link.href"
                  class="subheading mx-3"
                  target="_blank"
                  style="color:black"
                >{{ link.text }}<br></a>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          </v-flex>
        </v-layout>
        </v-img>
      </v-flex>

      <v-flex xs4 mb-5  ><v-img src="../assets/7.jpg" > 
        <h2 class="headline font-weight-bold mb-3">运营管理系统</h2>

        <v-layout justify-center row wrap>
          <v-flex d-flex>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title>
                <a
                  v-for="(eco, i) in operations"
                  :key="i"
                  :href="eco.href"
                  class="subheading mx-3"
                  target="_blank"
                    style="color:burlywood"
                >{{ eco.text }}<br></a>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          </v-flex>
        </v-layout>
        </v-img>
      </v-flex>
      <v-flex xs12>
  <v-footer
    style="background-color:darkgray"
  >
      <v-card-title  style="width:100%">
          <v-flex xs4>
        <strong class="subheading" style="color:antiquewhite">沈阳市苜蓿草科技有限公司</strong>
          </v-flex>
          <v-flex xs8>
         <span style="color:black;msrgin-right'50px'" ><h5>  电话：024-62571157   地址：沈阳市皇姑区万众商务大厦14-5   邮箱： eastwill.net@126.com</h5></span>
          </v-flex>
      </v-card-title>
       
  </v-footer>
 
  </v-flex>
    </v-layout>
  </v-container> 
</template>

<script>
import a from "../assets/2.jpg";
import b from "../assets/2.jpeg";
import c from "../assets/3.jpg";
import d from "../assets/4.jpg";
export default {
  data: () => ({
    items: [
          {
            src: b,
          },
          {
            src:a,
          },
          {
            src: c,
          },
          {
            src: d,
          },
        ],
    operations: [
      {
        text: "人力资源管理",
        href: "http://www.cloveropen.com"
      },
      {
        text: "设备材料管理",
        href: "https://cloveropen.app-hos.com:9092/"
      },
      {
        text: "物资供应管理",
        href: "https://cloveropen.app-hos.com:9093/"
      },
      {
        text: "预算管理",
        href: "http://www.cloveropen.com"
      },
       {
        text: "财务管理",
        href: "https://cloveropen.app-hos.com:9090/"
      },
      {
        text: "药品管理",
        href: "https://cloveropen.app-hos.com:9091/"
      }
    ],
    healthCare: [
      {
        text: "食源性疾病上报系统接口",
        href: "http://www.cloveropen.com"
      },
       {
        text: "院感/传染病管理系统",
        href: "http://www.cloveropen.com"
      },
      {
        text: "医疗保险/新农合接口",
        href: "http://www.cloveropen.com"
      },
      {
        text: "职业病管理系统接口",
        href: "http://www.cloveropen.com"
      },
      {
        text: "科研教学管理系统",
        href: "http://www.cloveropen.com"
      },
      {
        text: "门急诊收费系统",
        href: "https://cloveropen.app-hos.com:9081/"
      },
      {
        text: "住院收费系统",
        href: "https://cloveropen.app-hos.com:9082"
      },
      {
        text: "护理管理系统",
        href: "https://cloveropen.app-hos.com:9085"
      },
      {
        text: "医务管理系统",
        href: "http://www.cloveropen.com"
      },
     
      {
        text: "病案管理系统",
        href: "http://www.cloveropen.com"
      }
    ],
    clinicSrv: [
      {
        text: "电子病历书写与管理",
        href: "https://cloveropen.app-hos.com:9087"
      },
      {
        text: "超声/内镜/病理管理",
        href: "http://www.cloveropen.com"
      },
      
       {
        text: "门诊医生工作站",
        href: "https://cloveropen.app-hos.com:9083"
      },
      {
        text: "住院医生工作站",
        href: "https://cloveropen.app-hos.com:9084"
      },
      {
        text: "住院护士工作站",
        href: "https://cloveropen.app-hos.com:9085"
      },
      {
        text: "门急诊挂号收费",
        href: "https://cloveropen.app-hos.com:9081/"
      },
      {
        text: "住院病人入出转",
        href: "https://cloveropen.app-hos.com:9082"
      },
      {
        text: "合理用药管理",
        href: "http://www.cloveropen.com"
      },
      {
        text: "手术麻醉管理",
        href: "https://cloveropen.app-hos.com:9089"
      },
      {
        text: "临床路径管理",
        href: "http://www.cloveropen.com"
      },
      {
        text: "医学影像(PACS)",
        href: "http://www.cloveropen.com"
      },
      {
        text: "临床检验(LIS)",
        href: "http://www.cloveropen.com"
      },
      {
        text: "分诊管理",
        href: "http://www.cloveropen.com"
      },
      
      {
        text: "输血管理",
        href: "https://cloveropen.app-hos.com:9088"
      },
      {
        text: "重症监护",
        href: "https://cloveropen.app-hos.com:9095"
      },
      {
        text: "心电管理",
        href: "http://www.cloveropen.com"
      },
      {
        text: "体检管理",
        href: "http://www.cloveropen.com"
      }
    ]
  })
};
</script>
<style lang="scss" scoped>
.mb-3{
  color:darkkhaki;
}
a{
  text-decoration: none;
  font-size: 20px
}
.mb-5{
  background-color: darkgray;
 
}

</style>