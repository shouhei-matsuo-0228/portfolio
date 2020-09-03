<template>
  <div class="profile-section">
    <div class="profile-image-wrapper">
      <img
        src="~/assets/profile.jpeg"
        alt="Profile Image"
        class="profile-image"
      />
    </div>
    <div class="profile-detail">
      福島県出身の松尾です。社会人歴は7年位です。新卒で証券会社に入社してリテール営業をしていました。その後にエンジニアに転職しました。最初は業務系のアプリを「VB」「Perl」で作ってましたが、ひょんなことから「Ruby」に出会いWEB系の企業に転職。その後なんやかんやありまして、現在はまちいろでWEBエンジニアとして働いています。
    </div>
  </div>
</template>

<style lang="sass" scoped>
.profile-section
  display: flex
  padding: 30px

  .profile-image-wrapper
    margin-right: 30px

    .profile-image
      border-radius: 300px

  .profile-detail
    font-size: 24px
    display: flex
    justify-content: center
    align-items: center
</style>
