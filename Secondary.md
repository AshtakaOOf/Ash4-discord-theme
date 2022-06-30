# css snippets that do not have any github

## message link
``` 
  .mention.wrapper-1ZcZW- {
    border-radius: 0;
    color: var(--old-blurple);
    background: var(--mention-10a);
    padding-bottom: 1px;
    padding-top: 1px;
    top: 1px;
}
.message-2CShn3.mentioned-Tre-dv .contents-2MsGLg .markup-eYLPri > .mention.wrapper-1ZcZW- {
    background: none;
    padding: 0;
}
.mention.wrapper-1ZcZW-:hover {
    text-decoration: underline;
    background: var(--mention-20a);
}
/*Role*/
.message-2CShn3.mentioned-Tre-dv .roleMention-11Aaqi {
    background: none !important;
    padding: 0;
}
/*Channel*/
.iconMentionText-1_WCtN {
    padding-bottom: 2px !important;
}
.mention.iconMentionText-1_WCtN, .message-2CShn3.mentioned-Tre-dv .contents-2MsGLg .markup-eYLPri > .mention.mention.iconMention-3WxjBe {
    border-radius: 0;
    color: var(--old-blurple);
    background: var(--mention-10a);
    padding: 0 2px 0 1.2rem;
    top: 0;
}
.mention.iconMentionText-1_WCtN:hover, .message-2CShn3.mentioned-Tre-dv .contents-2MsGLg .markup-eYLPri > .mention.mention.iconMention-3WxjBe:hover {
    text-decoration: underline;
    background: var(--mention-20a);
}

body {
  --old-blurple: #7289DA;
  --mention-10a: rgba(114,137,218,0.1);
  --mention-20a: rgba(114,137,218,0.2);
}
```
## Little Friend Request Fix
```
.panel-3DsHLr {
max-width: unset;
}
```

## Emoji selector slider
```
.chatContent-3KubbW .expression-picker-chat-input-button:nth-of-type(1),
.chatContent-3KubbW .expression-picker-chat-input-button:nth-of-type(2) {
  order: -3 !important;
  z-index: -1;
}

.chatContent-3KubbW .buttons-uaqb-5 .expression-picker-chat-input-button:nth-of-type(1) > button {
    animation: slideOut 0.6s forwards;
}

.chatContent-3KubbW .buttons-uaqb-5 .expression-picker-chat-input-button:nth-of-type(2) > button{
    animation: slideOut2 0.6s forwards;
}

.chatContent-3KubbW .buttons-uaqb-5:hover .expression-picker-chat-input-button:nth-of-type(1) > button{
    animation: slideIn .4s forwards;
    display: flex;
}

.chatContent-3KubbW .buttons-uaqb-5:hover .expression-picker-chat-input-button:nth-of-type(2) > button{
    animation: slideIn .4s forwards;
    display: flex;
}

@keyframes slideIn {
    from {right: -40px; display: none;}
    to {right: 0px; display: block;}
}

@keyframes slideOut {
    from {right: 0px; display: block;}
    to {right: -80px; position: fixed;}
}

@keyframes slideOut2 {
    from {right: 0px; display: block;}
    to {right: -99px; position: fixed;}
}

.chatContent-3KubbW .buttons-uaqb-5 {
    order: 3 !important;
}

.chatContent-3KubbW .buttons-uaqb-5 > .expression-picker-chat-input-button:nth-of-type(3) {
    order: -2 !important;
  background-color: var(--channeltextarea-background);
}
```

## Spotify tweak
``` 
/* Re-round Spotify Status Images */
.assetsLargeImageSpotify-17ME3M{border-radius:8px;}

## About me tweak
.clamped-2ZePhX {
  -webkit-line-clamp: unset;
}

## message bar tweak
.form-3gdLxP {
  padding: 0px;
}

.inner-NQg18Y {
  padding-top: 4px;
}

.channelTextArea-1VQBuV {
  margin-bottom: 0px;
}

.base-3bcbY3 {
  top: -24px;
  left: 0px;
  width: fit-content;
  padding-right: 9px;
  border-radius: 0 8px 0 0;
  background-color: var(--channeltextarea-background);
}

.scrollableContainer-15eg7h {
  border-radius: 0px;
  min-height: 53px;
}
```

## Edited message tweak
/* edited text */
.timestamp-p1Df1m:not(.timestampInline-_lS3aK, .timestampVisibleOnHover-9PEuZS) time::after {
        content: " (" attr(aria-label) ")";
        color: var(--text-muted);
        font-size: 0.625rem;
        font-weight: 400;
        line-height: 1;
        text-transform: lowercase;
}

.edited-1v5nT8:not(.message-translate-indicator) {
    display: none;
}

## Banner gradient
.header-3OsQeK {
  box-shadow: none;
}

.animatedContainer-2laTjx {
  box-shadow: none;
}

.animatedContainer-2laTjx::before {
  background: linear-gradient(transparent 0%, var(--background-secondary) 100%, transparent 0%);
  position: absolute;
  content: "";
  height: 20px;
  width: 100%;
  bottom: 0;
  z-index: 1;
}

## Bug fix 1
.messagesPopoutWrap-3zryHW{
  max-height:70vh !important;
  width:30vw;
}

## Role tweak
```
/** Optional */
@import "https://spinfish.github.io/css-snippets/snippets/filled-roles.css";

:root {
    /** Number of role columns */
    --roleslist-columns: 2;
}

.rolesList-1geHY1 {
    display: grid;
    grid-template-columns: repeat(var(--roleslist-columns), minmax(0, 1fr));
    background: var(--background-tertiary);
    padding: 12.5px;
    gap: 4.5px;
    border-radius: 8px;
    max-height: 150px;
    overflow: auto;
}
.rolesList-1geHY1::-webkit-scrollbar {
    width: 4.5px;
}
.rolesList-1geHY1::-webkit-scrollbar-thumb {
    border-radius: 8px;
    background-color: var(--background-modifier-hover);
}
.rolesList-1geHY1 > .role-2irmRk {
    margin: 0;
    justify-content: center;
}
.rolesList-1geHY1 .roleCircle-3xAZ1j {
    flex-shrink: 0;
}
.rolesList-1geHY1 .roleName-32vpEy {
    margin: auto;
}

.addButton-pcyyf6 {
    grid-column: 1 / span var(--roleslist-columns);
}
.addButton-pcyyf6::before {
    content: attr(aria-label);
    text-transform: capitalize;
}
.addButtonIcon-1NMJ8u {
    display: none;
}
```

## media tweak
```
/* Horizontally listed media */
[id*="message-accessories-"] {
    display: flex;
    flex-wrap: wrap;
}
[id*="message-accessories-"] > * {
    margin-right: .4em !important;
    min-height: 100% !important;
}
[id*="message-accessories-"] > div > a {
    display: flex;
    align-items: center;
    min-height: 100%;
    background-color: var(--background-secondary);
}
[id*="message-reactions"] {
    width: 100%;
}
```

## user toggle
```
/* Sidebar */
.members-3l0kz9 {
    height: 100%;
}
/* Channel header */
.toolbar-3_r2xA>.iconWrapper-2awDjA.selected-29KTGM:nth-of-type(4)~:last-child {
    margin-right: 56px;
}
/* Buttons */
.container-2Oqvgx>.tabs-1RhQha {
    height: 0;
    padding: 0;
    border: none;
}
.container-2Oqvgx>.tabs-1RhQha>.tab-FftSDB {
    font-size: 0;
    position: absolute;
    right: 6px;
    top: -36px;
    width: 40px;
    height: 24px;
    margin: 0 8px;
    padding: 0;
    z-index: 2;
    border-radius: 12px;
    background-color: hsl(218, calc(var(--saturation-factor, 1) * 4.6%), 46.9%) !important;
}
.container-2Oqvgx>.tabs-1RhQha>.tab-FftSDB::after {
    position: absolute;
    top: 3px;
    width: 18px;
    height: 18px;
    background-color: white;
    border-radius: 50%;
}
.container-2Oqvgx>.tabs-1RhQha>.tab-FftSDB:first-of-type::after {
    content: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='18px' height='18px' fill='rgb(114, 118, 125)'><path d='M9-1zm0 4.752a1.25 1.25 90 110 2.5a1.25 1.25 90 010-2.5zM12 14h-6v-2h2V9H7V7h2a1 1 90 011 1v4h2v2z'/></svg>");
    right: 3px;
}
.container-2Oqvgx>.tabs-1RhQha>.tab-FftSDB:last-of-type::after {
    content: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='18px' height='18px' fill='rgb(114, 118, 125)'><path d='M11.8 6.6C11.8 8.154 10.54 9.4 9 9.4C7.46 9.4 6.2 8.154 6.2 6.6C6.2 5.06 7.46 3.8 9 3.8C10.54 3.8 11.8 5.06 11.8 6.6ZM3.4 14.3C3.4 11.836 5.71 10.1 9 10.1C12.304 10.1 14.6 11.836 14.6 14.3V15H3.4V14.3Z'/></svg>");
    left: 3px;    
}
.container-2Oqvgx>.tabs-1RhQha>.tab-FftSDB.selected-g-kMVV {
    pointer-events: none;
    opacity: 0;
}
```

## Bug fix 2
```.audioMetadata-3zOuGv::before {
    min-width: 24px;
}
```

## Rounded user panel
```
/* Rounded User Panel */
.container-YkUktl {
         margin-right: 5px;
         margin-bottom: 10px;
         margin-left: 5px;
         border: 1px solid rgb(78, 78, 81); 
         border-radius: 20px;
         box-shadow: 0 0 3px 1px rgba(0, 0, 0, 0.483);
         background: rgba(0, 0, 0, 0.436); 
    }
.panels-3wFtMD {
         background-color: #00000000;
}
```
## Collapsing Voice Panel
```
.container-1zzFcN .actionButtons-2vEOUh {
  transition: 250ms ease-out;
  padding-top: 0px;
  opacity: 0;
  height: 0;
}
.container-1zzFcN:hover .actionButtons-2vEOUh {
  padding-top: 4px;
  height: 36px;
  opacity: 1;
}
```
## Shoshinsha newbies!
```
/* Shoshinsha symbol for new server members */
img.newMemberBadge-3PdStX, .iconContainer-11h7fa img {
    background-image: url(/assets/bd766f88fab518680708df9935b50e85.svg);
    padding: 20px 20px 0 0; 
    background-size:auto; 
    width:0px; 
    height: 0px;
}

.iconContainer-11h7fa img {
    padding: 40px 40px 0 0; 
}
```
## Timestamp overhaul
```
.timestamp-6-ptG3 {
  border-radius: 7px; 
  padding: 2.5px;

}

.timestamp-6-ptG3::before {
  content: url("data:image/svg+xml,%3Csvg width='12px' height='12px' role='img' fill='white' viewBox='0 0 520 520' xmlns='http://www.w3.org/2000/svg'%3E%3Ctitle%3EDiscord%3C/title%3E%3Cpath d='M256,8C119,8,8,119,8,256S119,504,256,504,504,393,504,256,393,8,256,8Zm92.49,313h0l-20,25a16,16,0,0,1-22.49,2.5h0l-67-49.72a40,40,0,0,1-15-31.23V112a16,16,0,0,1,16-16h32a16,16,0,0,1,16,16V256l58,42.5A16,16,0,0,1,348.49,321Z'/%3E%3C/svg%3E");
    margin: 4px;
    position: relative;
    top: 1.5px;
}

.theme-light .timestamp-6-ptG3::before {
  filter: invert(87%); 
}
```
## Better profile modal
```
:root{
    --radius:4px!important;
    --roles-colums:135px 135px;
    --popout-backdrop:rgba(0,0,0,0.562);
    --popout-backdrop-blur:blur(1.5px);
    --popout-modal-badges-style:30px;
    --popout-badges-radius:0 12px 12px 0;
    --popout-badges-transparency:rgba(2,2,2,0.5);
    --avatar-profile-banner-blur:blur(0.9px);
    --avatar-profile-banner-opacity:.4;
    --popout-backdrop:rgba(0,0,0,0.562);
    --popout-backdrop-blur:blur(1.5px)
}
.backdrop-2ByYRN{background-color:var(--popout-backdrop)!important;backdrop-filter:var(--popout-backdrop-blur)!important}
.profileBannerPremium-KD60EB,.profileBanner-1owKI5{height:280px;filter:var(--avatar-profile-banner-blur);opacity:var(--avatar-profile-banner-opacity);margin:15px;margin-bottom:0;border-radius:var(--radius)}
.avatar-3QF_VA{position:absolute!important;top:-220px!important;left:40.2%!important;border:0 solid var(--background-floating)!important;background-color:var(--background-floating)!important}
.nameTag-2Nlmsy{top:145px;left:185px;position:fixed;width:200px!important;max-width:200px!important}
.badgeList-2aoHPw{display:grid;flex-direction:column;grid-template-columns:var(--popout-modal-badges-style);left:14px;top:74px;width:max-content;background-color:var(--popout-badges-transparency);border-radius:var(--popout-badges-radius);padding:4px;position:fixed}
.nameTag-2Nlmsy,.nameTag-2Nlmsy .discriminator-1bqsd3,.tabBarContainer-sCZC4w{display:flex;justify-content:center;text-align:center}
.customStatusActivity-WKWGD-{padding:0 16px 8px}
.top-K_jibn .item-3XjbnG{background-color:var(--background-secondary);padding:8px;border-bottom:0 solid transparent;border-radius:var(--radius);margin:10px 5px}
.top-K_jibn .item-3XjbnG:hover{background-color:var(--alt-color2)}
.tabBarContainer-sCZC4w{padding-top:0;margin-top:0!important;padding-bottom:10px;border-bottom:1px solid var(--background-modifier-accent)}
.empty-2zcusz{align-content:center;align-items:center;text-align:center;width:560px}
.relationshipButtons-3ByBpj{position:fixed;top:30px;right:25px}
@media only screen and (min-height: 1235px) {
.body-1Ukv50{max-height:680px!important;min-height:680px!important}
}
@media only screen and (max-height: 1240px) {
.body-1Ukv50{max-height:680px!important;min-height:470px!important}
}
@media only screen and (max-height: 1030px) {
.body-1Ukv50{max-height:470px!important;min-height:320px!important}
}
@media only screen and (max-height: 830px) {
.body-1Ukv50{max-height:320px!important;min-height:130px!important}
}
.customStatusText-_4TbWr{padding:8px;margin-top:55px!important;border-radius:var(--radius);align-content:center;align-items:center;text-align:center;background-color:var(--background-secondary)}
.customStatusText-_4TbWr::before{content:"STATUS";background-color:var(--background-secondary-alt);padding:8px;position:absolute!important;left:15px!important;top:305px!important;border-radius:var(--radius);color:var(--header-secondary)!important;font-weight:700;font-size:13px;text-transform:uppercase!important;width:553px!important;align-content:center;align-items:center;text-align:center}
.userInfoSectionHeader-2mYYun{padding:8px;border-radius:var(--radius);align-content:center;align-items:center;text-align:center;background-color:var(--background-secondary-alt)}
.userInfoText-2MFCmH{padding:8px;margin-top:15px;border-radius:var(--radius);align-content:center;align-items:center;text-align:center;background-color:var(--background-secondary)}
.note-3M15gE textarea{width:560px;margin-left:4px;margin-top:15px;border-radius:var(--radius);align-content:center;align-items:center;text-align:center;background-color:var(--background-secondary);padding:8px 0}
.connectedAccounts-1YaT2t::before{content:"Connected Accounts";background-color:var(--background-secondary-alt);padding:8px;margin-top:8px;border-radius:var(--radius);color:var(--header-secondary)!important;font-weight:700;font-size:13px;text-transform:uppercase!important;width:543px;align-content:center;align-items:center;text-align:center}
.userInfoSection-2u2hir+.userInfoSection-2u2hir{border-top:0 solid var(--background-modifier-accent)!important}
.connectedAccount-1xKpli{padding:8px;margin-top:15px;border-radius:var(--radius);align-content:center;align-items:center;text-align:center;background-color:var(--background-secondary)}
.connectedAccounts-1YaT2t{width:560px!important}
.listScroller-entkMk{display:grid!important;flex-direction:column!important;grid-template-columns:285px 285px;border-radius:var(--radius);padding:4px;height:auto;align-content:center;align-items:center;margin-top:10px;margin-left:10px}
.listRow-2nO1T6{height:50px;background-color:var(--background-secondary);border-radius:var(--radius);padding:4px}
.listAvatar-2bU5Uh,.listRowContent-PEmSWj{margin-left:10px;padding:1px}
.lookFilled-yCfaCM.colorGreen-3y-Z79{border-radius:var(--radius)}
```
