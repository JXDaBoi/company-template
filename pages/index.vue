<template>
  <div class="relative">
    <div class="h-screen">
      <div class="flex flex-col">
        <!-- 
          Header Content ( Landing Page )

          PARAMETERS
          :imgURL (URL for Background)
          :header_txt ( Header Text )
          :second_header ( Header 2 Text)
          :descriptions ( Descriptions )
        -->
        <HeaderContent
          imgURL="https://64.media.tumblr.com/659df02b71ed0fca9725f28cc671356b/tumblr_plbt6hv1ij1wuv92g_540.png"
          header_txt="王阿姨团队"
          second_header="想月入过万吗？"
          descriptions="加入我们的团队就对了"
        ></HeaderContent>
        <!-- 
          About Content 

          PARAMETERS
          :imgURL ( URL for about us )
        -->
        <AboutContent
          imgURL="https://64.media.tumblr.com/659df02b71ed0fca9725f28cc671356b/tumblr_plbt6hv1ij1wuv92g_540.png"
        >
          <template v-slot:about>加入我们的团队就可以少奋斗一世纪， 别等了 :)</template>
        </AboutContent>

        <ServiceContent>
          <template v-slot:services>
            <!-- 

              Service 

              PARAMETERS

              :imgURL (image url)
            -->
            <Service imgURL="/img/icon1.png" title="帮阿姨和叔叔换灯泡">
              <template v-slot:content>就纯粹帮阿姨们和叔叔们换灯泡，以换得肉体和心灵上的回报</template>
            </Service>

            <Service imgURL="/img/icon2.png" title="陪阿姨和叔叔聊天">
              <template v-slot:content>就纯粹和阿姨们和叔叔们吹水，聊聊心事，顺便可以得到心灵上的辅导</template>
            </Service>
          </template>
        </ServiceContent>

        <!-- 
          Portfolio
        -->
        <PortfolioContent>
          <template v-slot:portfolio>
            <!-- 
              Project

              PARAMETERS
              :imgURL ( img URL for Project )
              :name ( Name of the Project )
              :project ( Name of Project Type)
              :projectURL ( Link Address to project)
            -->
            <Project
              imgURL="https://64.media.tumblr.com/659df02b71ed0fca9725f28cc671356b/tumblr_plbt6hv1ij1wuv92g_540.png"
              name="Project Name"
              project="Project Type"
              projectURL="https://google.com"
            />
          </template>
        </PortfolioContent>
        <ContactContent
          address="Level 11, Menara KEN TTDI, No.37 Jalan Burhanuddin Helmi, Taman Tun Dr. Ismail"
          email="support@thelead.io"
          phone="6016-473 7281"
          imgURL="/img/lead-white-logo.png"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>