<template>
  <div>
    <complete-chat />
    <!-- Start of Chat -->
    <!-- <div class="chat" id="chat1">
      <div class="top">
        <top-bar-menu-component />
      </div>
      <div class="content" id="content">
        <div class="container">
          <div class="col-md-12">
            <div class="date">
              <hr />
              <span>Yesterday</span>
              <hr />
            </div>
            <div class="message">
              <img
                class="avatar-md"
                src="img/avatars/avatar-female-5.jpg"
                data-toggle="tooltip"
                data-placement="top"
                title="Keith"
                alt="avatar"
              />
              <div class="text-main">
                <div class="text-group">
                  <div class="text">
                    <p>We've got some killer ideas kicking about already.</p>
                  </div>
                </div>
                <span>09:46 AM</span>
              </div>
            </div>
            <div class="message me">
              <div class="text-main">
                <div class="text-group me">
                  <div class="text me">
                    <p>Can't wait! How are we coming along with the client?</p>
                  </div>
                </div>
                <span>11:32 AM</span>
              </div>
            </div>
            <div class="message">
              <img
                class="avatar-md"
                src="img/avatars/avatar-female-5.jpg"
                data-toggle="tooltip"
                data-placement="top"
                title="Keith"
                alt="avatar"
              />
              <div class="text-main">
                <div class="text-group">
                  <div class="text">
                    <p>
                      Coming along nicely, we've got a draft for the client
                      quarries completed.
                    </p>
                  </div>
                </div>
                <span>02:56 PM</span>
              </div>
            </div>
            <div class="message me">
              <div class="text-main">
                <div class="text-group me">
                  <div class="text me">
                    <p>Roger that boss!</p>
                  </div>
                </div>
                <div class="text-group me">
                  <div class="text me">
                    <p>
                      I have already started gathering some stuff for the mood
                      boards, excited to start!
                    </p>
                  </div>
                </div>
                <span>10:21 PM</span>
              </div>
            </div>
            <div class="message">
              <img
                class="avatar-md"
                src="img/avatars/avatar-female-5.jpg"
                data-toggle="tooltip"
                data-placement="top"
                title="Keith"
                alt="avatar"
              />
              <div class="text-main">
                <div class="text-group">
                  <div class="text">
                    <p>
                      Great start guys, I've added some notes to the task. We
                      may need to make some adjustments to the last couple of
                      items - but no biggie!
                    </p>
                  </div>
                </div>
                <span>11:07 PM</span>
              </div>
            </div>
            <div class="date">
              <hr />
              <span>Today</span>
              <hr />
            </div>
            <div class="message me">
              <div class="text-main">
                <div class="text-group me">
                  <div class="text me">
                    <p>
                      Well done all. See you all at 2 for the kick-off meeting.
                    </p>
                  </div>
                </div>
                <span>10:21 PM</span>
              </div>
            </div>
            <div class="message">
              <img
                class="avatar-md"
                src="img/avatars/avatar-female-5.jpg"
                data-toggle="tooltip"
                data-placement="top"
                title="Keith"
                alt="avatar"
              />
              <div class="text-main">
                <div class="text-group">
                  <div class="text">
                    <div class="attachment">
                      <button class="btn attach">
                        <i class="material-icons md-18">insert_drive_file</i>
                      </button>
                      <div class="file">
                        <h5><a href="#">Tenacy Agreement.pdf</a></h5>
                        <span>24kb Document</span>
                      </div>
                    </div>
                  </div>
                </div>
                <span>11:07 PM</span>
              </div>
            </div>
            <div class="message me">
              <div class="text-main">
                <div class="text-group me">
                  <div class="text me">
                    <p>
                      Hope you're all ready to tackle this great project. Let's
                      smash some Brand Concept & Design!
                    </p>
                  </div>
                </div>
                <span><i class="material-icons">check</i>10:21 PM</span>
              </div>
            </div>
            <div class="input">
              <typing-component />
            </div>
          </div>
        </div>
      </div>
      <input-component />
    </div>-->
    <!-- End of Chat -->
    <!-- Start of Call 
    <call-component /> -->
    <!-- End of Call -->
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import TypingComponent from "./TypingComponent.vue";
import InputComponent from "./InputMessageComponent.vue";
import TopBarMenuComponent from "./TopBarMenuComponent.vue";
import CompleteChat from "./CompleteChat.vue";
import SockJS from "sockjs-client";
import Stomp, { Client } from "webstomp-client";

interface Message {
  content: string;
  count: number;
}

let stompChatClient: Client;

const ChatComponent = defineComponent({
  name: "chatcomponent",
  components: {
    CompleteChat,
    //TopBarMenuComponent,
    //InputComponent,
  },
});

export default ChatComponent;
</script>
