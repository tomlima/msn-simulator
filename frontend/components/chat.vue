<template>
  <div class="chat" id="chat">
    <div class="tabs">
      <button class="tabbutton">
        <img
          class="status-icon"
          src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/status/busy.png"
          alt="status"
        />
        <span class="name"><b>Alto</b></span>
      </button>
      <button class="tabbutton">
        <img
          class="status-icon"
          src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/status/away.png"
          alt="status"
        />
        <span class="name">Duck</span>
      </button>
      <button class="tabbutton">
        <img
          class="status-icon"
          src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/status/online.png"
          alt="status"
        />
        <span class="name">jake</span>
      </button>
    </div>
    <div class="header">
      <div id="info">
        <img
          id="chaticon"
          src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/61.ico"
        />
        <div id="text">
          <span id="name">Alto</span>
          <span id="message">Wow, this is cool =) &lt;root@altodev.pw&gt;</span>
        </div>
      </div>
      <div id="navbars">
        <ul class="chatnav" id="left">
          <button
            class="aerobutton chataction"
            style="background:url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1441.png) no-repeat center;"
          ></button>
          <button
            class="aerobutton chataction"
            style="background:url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1444.png) no-repeat center;"
          ></button>
          <button
            class="aerobutton chataction"
            style="background:url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1447.png) no-repeat center;"
          ></button>
          <button
            class="aerobutton chataction"
            style="background:url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1442.png) no-repeat center;"
          ></button>
          <button
            class="aerobutton chataction"
            style="background:url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1443.png) no-repeat center;"
          ></button>
          <button
            class="aerobutton chataction"
            style="background:url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/326.png) no-repeat center;"
          ></button>
        </ul>
        <ul class="chatnav" id="right">
          <button class="aerobutton chataction smallarrowbtn" id="chatnav-expand">
            <img
              src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1489.png"
              style="height: 16px;"
            />
            <img
              class="arrowdown"
              src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/general/small_arrow.svg"
            />
          </button>
          <button
            class="aerobutton chataction"
            style="background:url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/329.png) no-repeat center;"
          ></button>
        </ul>
      </div>
    </div>
    <div class="conversation">
      <div id="messages">
        <div id="recieve">
          <div class="alerts">
            <img
              src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1539.png"
              alt=""
            />
            <p class="alerttext">Alto is Busy and may not reply</p>
          </div>
          <textarea class="chattext" id="display" readonly></textarea>
        </div>
        <div id="handle"></div>
        <div id="send">
          <ul id="options">
            <button class="aerobutton textoption smallarrowbtn">
              <img src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/412.png" />
              <img
                class="arrowdown"
                src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/general/small_arrow.svg"
              />
            </button>
            <button class="aerobutton textoption smallarrowbtn">
              <img src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1487.png" />
              <img
                class="arrowdown"
                src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/general/small_arrow.svg"
              />
            </button>
            <button
              class="aerobutton textoption noarrow"
              style="background: url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/414.png) no-repeat center;"
            ></button>
            <button
              class="aerobutton textoption noarrow"
              style="background: url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/992.png) no-repeat center;"
            ></button>
            <button
              class="textoption"
              style="background: url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/20204.png) no-repeat center; border: none;"
            ></button>
          </ul>
          <textarea class="chattext" id="write" placeholder="Type your message here..."></textarea>
          <div id="bottomtabs">
            <button class="editortab selected">
              <img src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/963.png" />
            </button>
            <button class="editortab unselected">
              <img src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/961.png" />
            </button>
            <div>
              <button id="sendbutton" disabled>Send</button>
              <button id="search" disabled></button>
            </div>
          </div>
        </div>
      </div>
      <div id="avatars">
        <div id="topavatar">
          <img
            class="avatar"
            src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1531.png"
            alt=""
          />
          <img
            class="frame"
            src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/background/frame_96.png"
          />
          <div class="avatarnav">
            <button
              class="aerobutton avataraction"
              style="background: url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/268.png) no-repeat center;"
            ></button>
            <button
              class="aerobutton avataraction"
              style="background: url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1457.png) no-repeat center; float: right;"
            ></button>
          </div>
        </div>
        <div id="bottomavatar">
          <img
            class="avatar"
            src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/01CAT.jpg"
            alt=""
          />
          <img
            class="frame"
            src="https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/background/frame_96.png"
          />
          <div class="avatarnav">
            <button
              class="aerobutton avataraction"
              style="background: url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1457.png) no-repeat center; float: right;"
            ></button>
          </div>
        </div>
      </div>
      <div id="expand">
        <button class="expandbutton"></button>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.chat {
  background-color: #ecf6f9;
  border: thin solid #707070;
  border-radius: 8px;
  box-shadow: 0 0 5px #00000050;
  transform: translateY(150%);
  transition: all 1s ease;
  &.is--open {
    transition: all 1s ease;
    transform: translateY(0);
  }
}

.aerobutton {
  background-color: transparent;
  border: 2px solid transparent;
}
.aerobutton:hover {
  border-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/general/aerobutton_border.png')
    2 round;
}
.aerobutton:active {
  border-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/general/aerobutton_border_down.png')
    2 round;
}

.emoticon {
  margin: 0 3px;
}

.smallarrowbtn {
  display: flex;
  flex-direction: row;
  overflow: hidden;
  align-items: center;
}
.arrowdown {
  height: 5px;
  margin-left: 4px;
}

.alerts {
  display: flex;
  align-items: center;
  height: 19px;
  background-color: white;
  border: thin solid #bed6e0;
  border-bottom: none;
}
.alerttext {
  margin: 0;
  margin-left: 3px;
}

#contacts {
  background-color: white;
  float: left;
  width: 30%;
  min-width: 274px;
  height: 100%;
  position: relative;
}

#contacts > .header {
  background-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/background/msgres_fullheader.png');
  background-repeat: no-repeat;
  background-size: 100% 100%;
  height: 95px;
  width: 100%;
}
.titlebar {
  padding: 6px;
  padding-bottom: 5px;
  height: 28px;
  display: flex;
  flex-direction: row;
  height: fit-content;
}
#title {
  height: 10px;
  margin-top: 4px;
  margin-left: 4px;
}

.user-info {
  display: flex;
  height: 69px;
  width: 100%;
  box-sizing: border-box;
  padding: 8px 14px;
}
#frame {
  height: 62px;
  width: auto;
  position: absolute;
  top: 31px;
  left: 9px;
}
#avatar {
  height: 48px;
  width: auto;
  border-radius: 2px;
}

.profile {
  margin: auto;
  margin-left: 14px;
  margin-top: 3px;
  height: 100%;
}
#user {
  padding: 0;
  height: fit-content;
  display: flex;
  text-align: start;
  align-items: center;
}
#user > h3 {
  font-size: 10pt;
  font-weight: 600;
  color: white;
  margin: 0;
}
#status {
  margin: 0;
  font-size: 8pt;
  color: #b9dde7;
  margin-left: 8px;
}

#message {
  padding: 0;
  margin: 0;
  height: fit-content;
  display: flex;
  text-align: start;
  align-items: center;

  color: #b9dde7;
  padding-top: 2px;
  padding-bottom: 3px;
  font-size: 8pt;
}
.arrowcontacts {
  margin-left: 8px;
  fill: #b9dde7 !important;
}

#contactsnav {
  background-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/background/msgres_navbar.png');
  background-size: 100% 100%;
  overflow: hidden;
  display: flex;
  flex-direction: row;
  height: 31px;
  padding: 0;
  box-shadow: 0px 1px 2px #00000077;
}
.iconbar {
  list-style: none;
  width: 50%;
  margin: 0;
  padding: 3px 8px 2px 8px;
}
.contactaction {
  height: 25px;
  width: 28px;
  margin: 0 2px;
  marker: none;
}
#left > .contactaction {
  float: left;
}
#right > .contactaction {
  float: right;
}

.search {
  display: flex;
  flex-direction: row;
  overflow: hidden;
  height: 38px;
  padding: 8px 8px 8px 7px;

  border-bottom: thin solid #e2eaf3;
}
#contact-search {
  font-size: 8pt;
  height: 23px;
  width: 100%;
  padding: 8px;
  margin-right: 7px;

  border: thin solid #c7c7c7;
  box-shadow: inset 0 0 3px #0000002a;
}
#contact-search:focus {
  border: thin solid #52c9fd;
  box-shadow: 0 0 6px #52cafdbe;
}

.searchbar-btn {
  height: 23px;
  width: 22px;
  border: 2px solid transparent;
}
.searchbar-btn:hover {
  border-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/button_border.png') 2 round;
}
.searchbar-btn:active {
  border-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/button_border_down.png') 2
    round;
}

.listitem {
  border: none;
  font-size: 8pt;
  text-align: start;
  height: 19px;
  width: 100%;
  overflow: hidden;
  text-overflow: ellipsis;
  background-color: white;
}
.listitem:focus {
  background-color: #d2eaf6;
}
.arrow {
  width: 9px;
  height: 9px;
  margin-right: 2px;
  background: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/arrows.png') 0 0;
}

.contact {
  padding-left: 19px;
  display: flex;
  flex-direction: row;
  align-items: center;
}
.status-icon {
  height: 100%;
  box-sizing: content-box;
}
.contact-text {
  margin: 0;
  text-anchor: middle;
  display: inline-block;

  text-overflow: ellipsis;
}
.message {
  overflow: hidden;
  white-space: nowrap;
}

#footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  margin: 0;
  padding: 5px 10px;
  background-color: #ecf6f9;
  border-radius: 0 0 8px 8px;
  border-top: thin solid #bed6e0;
}
#ad {
  display: block;
  margin: 10px auto;
}

#chat {
  height: 100%;
  width: 100%;
  min-width: 420px;
  margin-left: 8px;
  display: flex;
  flex-direction: column;
}
.tabs {
  height: 27px;
  padding: 2px;
  overflow: hidden;
  display: flex;
  flex-direction: row;
}
.tabbutton {
  height: 23px;
  width: 100%;
  min-width: 100px;

  margin: 0 2px;
  padding: 0 5px;
  border: thin solid #b8bdbd;
  border-radius: 6px 6px 0 0;

  background-color: #eff9f9;
  display: flex;
  flex-direction: row;
}
.tabbutton > .name {
  margin-top: 4px;
  text-anchor: middle;

  font-size: 8pt;
}

#chat > .header {
  border-top: thin solid #707070;
  image-rendering: pixelated;
  background-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/background/chat_header.png');
  background-size: 100% 100%;

  margin: 0;
  height: 77px;
  padding: 7px;

  box-shadow: 0px 1px 4px #00000057;
}
#info {
  display: flex;
}
#chaticon {
  height: 16px;
}
#text {
  display: flex;
  flex-direction: column;
  margin-left: 5px;
}
#text > #name {
  font-weight: bold;
  color: #333333;
}
#text > #message {
  color: #6f8a92;
  margin: 0;
}

#navbars {
  display: flex;
  flex-direction: row;
  margin-top: 3px;
  justify-content: space-between;
}
.chatnav {
  list-style: none;
  margin: 0;
  height: 33px;
  padding: 0;
}
.chataction {
  height: 100%;
  width: 33px;
  margin-left: 5px;
}
.chatnav > #left {
  width: 100%;
  min-width: 230px;
}
.chatnav > #right {
  width: 10%;
  min-width: 84px;
}
.chatnav#left > .chataction {
  float: left;
}
.chatnav#right > .chataction {
  float: right;
}
#chatnav-expand {
  padding: 0 3px;
  width: 40px;
}

.conversation {
  height: 100%;
  display: flex;
  padding: 10px;
  padding-right: 0;
  padding-bottom: 15px;
}
#messages {
  width: 100%;
  margin-right: 20px;
  display: flex;
  flex-direction: column;
}
.chattext {
  font-family: 'Tahoma', sans-serif;
  width: 100%;
  resize: none;
  border: thin solid #bed6e0;
}
#recieve {
  display: flex;
  flex-direction: column;
  height: 100%;
}
#display {
  margin: 0;
  height: 100%;
}

#handle {
  background-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/30417.png');
  background-repeat: no-repeat;
  background-position: center;
  height: 10px;
}

#send {
  display: flex;
  flex-direction: column;
  height: 200px;
}
#options {
  background-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/background/chat_editheader.png');
  border: thin solid #bed6e0;
  height: 29px;
  margin: 0;
  padding: 2px;
}
.textoption {
  height: 24px;
  width: auto;
  padding: 0 4px;
  float: left;
}
.noarrow {
  width: 32px;
}
#write {
  height: 100%;
  margin: 0;
  border-top: none;
  font-size: 10pt;
  padding: 4px 8px;
}
#bottomtabs {
  display: flex;
  justify-content: space-between;
  height: 24px;
  margin: 0;
  position: relative;
}
.editortab {
  width: 26px;
  height: 24px;
  margin: 0;
  padding: 0;

  display: flex;
  align-items: center;
  justify-content: center;

  border: thin solid #bed6e0;
  border-top: none;
  background-color: white;
}
.selected {
  position: absolute;
  bottom: 0;
  left: 0;
  height: 25px;

  border-top: 2px solid white;
}
.unselected {
  margin-left: 25px;
  border-left: none;
  background: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/editortab.png');
  image-rendering: pixelated;
}
.unselected:hover {
  background: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/editortab_down.png');
  background-size: 100% auto;
  image-rendering: pixelated;
}
#sendbutton {
  height: 21px;
  padding: 0 18px;
  margin: 2px;

  font-size: 8pt;
  color: #001563;

  background-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/general/button_inside.png');
  background-size: 100% auto;
  border: 3px solid transparent;
  border-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/general/button_border.png') 3;
}
#sendbutton:hover {
  border-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/general/button_border_focus.png')
    3;
}
#sendbutton:active {
  padding: 0 20px;
  filter: brightness(93%);
  border: thin solid #286088;
  border-radius: 3px;
  box-shadow: inset 1px 1px 2px #00000077;
}
#sendbutton:disabled {
  background-image: none;
  background-color: #f0f0f0;
  border-image: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/general/button_border_disabled.png')
    3;
  color: #c9c1c1;
}

#search {
  float: right;
  width: 23px;
  height: 21px;
  margin: 2px;

  background: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/653_multi.png') 0 0;
  border: none;
}
#search:hover {
  background: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/653_multi.png') -23px
    0;
}
#search:active {
  background: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/653_multi.png') -46px
    0;
}
#search:disabled {
  background: url('https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/653_multi.png') -69px
    0;
}
#avatars {
  height: 100%;
  position: relative;
}
#topavatar {
  position: relative;
}
#bottomavatar {
  position: absolute;
  bottom: 0;
}
.avatar {
  margin: 9px;
  height: 96px;
  border-radius: 2px;
}
.frame {
  position: absolute;
  top: 0;
  left: 0;
}
.avatarnav {
  height: 18px;
}
.avataraction {
  height: 100%;
}

#expand {
  margin-left: 18px;
}
.expandbutton {
  background: url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1450_multi.png) 0 0;
  background-repeat: no-repeat;
  border: none;

  padding: 0;
  width: 12px;
  height: 31px;
}
.expandbutton:hover {
  background: url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1450_multi.png) 26px 0;
}
.expandbutton:active {
  background: url(https://raw.githubusercontent.com/AndroidWG/WLMOnline/master/assets/chat-window/1450_multi.png) 13px 0;
}
</style>
