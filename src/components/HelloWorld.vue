<template>
  <v-container fluid grid-list-lg>
    <v-layout text-center wrap>
      <v-flex xs12>
        <v-img :src="require('../assets/logo.svg')" class="my-3" contain height="200"></v-img>
      </v-flex>

      <v-flex mb-4>
        <h1 class="display-2 font-weight-bold mb-3">智慧医院信息平台</h1>
        <p class="subheading font-weight-regular">以电子病历为核心的智慧医院信息平台</p>
      </v-flex>

      <v-flex mb-5 xs12>
        <h2 class="headline font-weight-bold mb-3">医疗管理系统</h2>

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
                >{{ next.text }}</a>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-layout>
      </v-flex>

      <v-flex xs12 mb-5>
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
                >{{ link.text }}</a>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          </v-flex>
        </v-layout>
      </v-flex>

      <v-flex xs12 mb-5>
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
                >{{ eco.text }}</a>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          </v-flex>
        </v-layout>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    operations: [
      {
        text: "人力资源管理",
        href: "http://www.openclover.com"
      },
      {
        text: "财务管理",
        href: "http://www.openclover.com"
      },
      {
        text: "药品管理",
        href: "http://www.openclover.com"
      },
      {
        text: "设备材料管理",
        href: "http://www.openclover.com"
      },
      {
        text: "物资供应管理",
        href: "http://www.openclover.com"
      },
      {
        text: "预算管理",
        href: "http://www.openclover.com"
      }
    ],
    healthCare: [
      {
        text: "门急诊收费系统",
        href: "http://www.openclover.com"
      },
      {
        text: "住院收费系统",
        href: "http://www.openclover.com"
      },
      {
        text: "护理管理系统",
        href: "http://www.openclover.com"
      },
      {
        text: "医务管理系统",
        href: "http://www.openclover.com"
      },
      {
        text: "院感/传染病管理系统",
        href: "http://www.openclover.com"
      },
      {
        text: "科研教学管理系统",
        href: "http://www.openclover.com"
      },
      {
        text: "病案管理系统",
        href: "http://www.openclover.com"
      },
      {
        text: "医疗保险/新农合接口",
        href: "http://www.openclover.com"
      },
      {
        text: "职业病管理系统接口",
        href: "http://www.openclover.com"
      },
      {
        text: "食源性疾病上报系统接口",
        href: "http://www.openclover.com"
      }
    ],
    clinicSrv: [
      {
        text: "门急诊挂号收费",
        href: "http://www.openclover.com"
      },
      {
        text: "住院病人入出转",
        href: "http://www.openclover.com"
      },
      {
        text: "分诊管理",
        href: "http://www.openclover.com"
      },
      {
        text: "门诊医生工作站",
        href: "http://www.openclover.com"
      },
      {
        text: "住院医生工作站",
        href: "http://www.openclover.com"
      },
      {
        text: "住院护士工作站",
        href: "http://www.openclover.com"
      },
      {
        text: "电子病历书写与管理",
        href: "http://www.openclover.com"
      },
      {
        text: "合理用药管理",
        href: "http://www.openclover.com"
      },
      {
        text: "临床检验(LIS)",
        href: "http://www.openclover.com"
      },
      {
        text: "医学影像(PACS)",
        href: "http://www.openclover.com"
      },
      {
        text: "超声/内镜/病理管理",
        href: "http://www.openclover.com"
      },
      {
        text: "手术麻醉管理",
        href: "http://www.openclover.com"
      },
      {
        text: "临床路径管理",
        href: "http://www.openclover.com"
      },
      {
        text: "输血管理",
        href: "http://www.openclover.com"
      },
      {
        text: "重症监护",
        href: "http://www.openclover.com"
      },
      {
        text: "心电管理",
        href: "http://www.openclover.com"
      },
      {
        text: "体检管理",
        href: "http://www.openclover.com"
      }
    ]
  })
};
</script>
