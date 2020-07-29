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
          imgURL="https://i.ibb.co/Mh4bTnR/halacious-t-Zc3vj-PCk-Q-unsplash.jpg"
          header_txt="PIZZAZ WEB STUDIO"
          second_header="YOUR CLIENTS WILL LOVE YOU!"
          descriptions="We create Unique Websites for an exciting & engaging user experience"
        ></HeaderContent>
        <!-- 
          About Content 

          PARAMETERS
          :imgURL ( URL for about us )
        -->
        <AboutContent
          imgURL="https://freepikpsd.com/wp-content/uploads/2019/10/about-us-logo-png-8-Transparent-Images.png"
        >
          <template
            v-slot:about
          >You need a website that can make you stand out from the crowd. We don't build just another boring website. PIZZAZ Web Studio's creations will engage your clients & keep them coming back for more.</template>
        </AboutContent>

        <ServiceContent>
          <template v-slot:services>
            <!-- 

              Service 

              PARAMETERS

              :imgURL (image url)
            -->
            <Service imgURL="/img/icon1.png" title="Web Design">
              <template v-slot:content>Creative solutions for your needs</template>
            </Service>

            <Service imgURL="/img/icon3.png" title="Web Development">
              <template v-slot:content>Get the website that your clients will LOVE!</template>
            </Service>

            <Service imgURL="/img/icon4.png" title="Web Conceptualisation">
              <template v-slot:content>Brainstorming for fresh & imaginative ideas</template>
            </Service>
            <Service imgURL="/img/icon2.png" title="SEO & Customer Engagement">
              <template
                v-slot:content
              >Search Engine Optimisation to make your website a customer magnet</template>
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
              imgURL="https://cdn.dribbble.com/users/723155/screenshots/4572417/git.jpg"
              name="PIZZAZ WEB STUDIO"
              project="Client Project 1"
              projectURL="https://github.com/MaxCodeXTC/company-template"
            />
            <Project
              imgURL="https://cdn.dribbble.com/users/723155/screenshots/4572417/git.jpg"
              name="PIZZAZ WEB STUDIO"
              project="Client Project 2"
              projectURL="https://github.com/MaxCodeXTC/company-template"
            />
            <Project
              imgURL="https://cdn.dribbble.com/users/723155/screenshots/4572417/git.jpg"
              name="PIZZAZ WEB STUDIO"
              project="Client Project 3"
              projectURL="https://github.com/MaxCodeXTC/company-template"
            />
            <Project
              imgURL="https://cdn.dribbble.com/users/723155/screenshots/4572417/git.jpg"
              name="PIZZAZ WEB STUDIO"
              project="Client Project 4"
              projectURL="https://github.com/MaxCodeXTC/company-template"
            />
          </template>
        </PortfolioContent>
        <ContactContent
          address="Level 88, Menara Towering Heights, No.88 Jalan Kaya Raya, Taman Bukit Emas"
          email="engage@pizzaz.com.my"
          phone="6016-888 8088"
          imgURL="https://www.logolynx.com/images/logolynx/99/99ea79e039ed844020667ed3ed9f1544.png"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: "PIZZAZ Web Creations"
    };
  }
};
</script>