<template>
  <aside
    class="hidden xl:block w-64 max-h-screen z-20 overflow-auto no-scrollbar fixed top-0 pt-12 bg-white"
  >
    <!--first section-->
    <SidebarSection>
      <ul>
        <SidebarItem label="Home" icon="home" is-active />
        <SidebarItem label="Trending" icon="fire" />
        <SidebarItem label="Subscriptions" icon="collection" />
      </ul>
    </SidebarSection>
    <!--second section-->
    <SidebarSection>
      <ul>
        <SidebarItem label="Library" icon="library" />
        <SidebarItem label="History" icon="history" />
      </ul>
    </SidebarSection>
    <!--third section Sing In text + signInButton-->
    <SidebarSection class="px-8 py-4 border-b leading-5 font-medium">
      <span class="text-sm">Sign in to like videos, comment and subscribe</span>
      <ButtonLogin class="mt-2" />
    </SidebarSection>
    <!--fourth section-->
    <SidebarSection>
      <SidebarSectionHeading title="Best Of YouTube" />
      <ul>
        <SidebarItem label="Music" icon="musicNote" />
        <SidebarItem label="Sports" icon="heart" />
        <SidebarItem label="Gaming" icon="puzzle" />
        <SidebarItem label="Movies" icon="movie" />
        <SidebarItem label="News" icon="news" />
        <SidebarItem label="Live" icon="liveStatus" />
        <SidebarItem label="360&deg; Video" icon="camera" />
      </ul>
    </SidebarSection>
    <!--fifth section-->
    <SidebarSection>
      <ul>
        <SidebarItem label="Browse channels" icon="plus" fill />
      </ul>
    </SidebarSection>
    <!--sixth section-->
    <SidebarSection>
      <SidebarSectionHeading title="more from youtube" />
      <ul>
        <!--Это лого, которого нет в icons.ts так что не трогаем иначе никак(ну можно но лень)-->
        <li>
          <a
            href="/"
            class="flex items-center px-6 py-2 text-sm hover:bg-gray-100"
          >
            <svg
              class="w-6 h-6 text-gray-700 mr-6"
              version="1.1"
              id="Layer_1"
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              viewBox="0 0 461.001 461.001"
              xml:space="preserve"
            >
              <g>
                <path
                  style="fill: #374151"
                  d="M365.257,67.393H95.744C42.866,67.393,0,110.259,0,163.137v134.728
            		c0,52.878,42.866,95.744,95.744,95.744h269.513c52.878,0,95.744-42.866,95.744-95.744V163.137
            		C461.001,110.259,418.135,67.393,365.257,67.393z M300.506,237.056l-126.06,60.123c-3.359,1.602-7.239-0.847-7.239-4.568V168.607
            		c0-3.774,3.982-6.22,7.348-4.514l126.06,63.881C304.363,229.873,304.298,235.248,300.506,237.056z"
                />
              </g>
            </svg>
            <span>YouTube premium</span>
          </a>
        </li>
        <SidebarItem label="Live" icon="live" />
      </ul>
    </SidebarSection>
    <!--seventh section-->
    <SidebarSection>
      <ul>
        <SidebarItem label="Settings" icon="settings" />
        <SidebarItem label="Report history" icon="flag" />
        <SidebarItem label="Help" icon="questionMark" />
        <SidebarItem label="Send feedback" icon="message" />
      </ul>
    </SidebarSection>
    <!--SidebarFooter section-->
    <SidebarSection class="px-6 py-4 text-sm font-semibold space-y-4">
      <TheFooter />
    </SidebarSection>
  </aside>
</template>

<script setup lang="ts">
import SidebarSection from './SidebarSection.vue'
import SidebarItem from './SidebarItem.vue'
import SidebarSectionHeading from './SidebarSectionHeading.vue'
import ButtonLogin from './ButtonLogin.vue'
import TheFooter from './TheFooter.vue'
</script>

<style scoped></style>
