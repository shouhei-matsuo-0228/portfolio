<template>
  <div class="main-container-outer">
    <Jumbotron header="松尾のPortfolio" sub-text="Webエンジニア" />

    <div class="main-container-inner">
      <ContentWrapper heading="プロフィール">
        <ProfileSection />
      </ContentWrapper>

      <ContentWrapper heading="スキル">
        <SkillSection
          :title="skillTypes.frontend.title"
          :fields="skillTypes.frontend.fields"
          :skills="skillTypes.frontend.skills"
        />
        <SkillSection
          :title="skillTypes.backend.title"
          :fields="skillTypes.backend.fields"
          :skills="skillTypes.backend.skills"
        />
        <SkillSection
          :title="skillTypes.other.title"
          :fields="skillTypes.other.fields"
          :skills="skillTypes.other.skills"
        />
      </ContentWrapper>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      // TODO: 別ファイルで持っておきたい。どこにファイル作るのが正解なのか。
      skillTypes: {
        frontend: {
          title: 'フロントエンド',
          fields: [
            { key: 'name', label: '技術' },
            { key: 'period', label: '経験年数' },
          ],
          skills: [
            { name: 'HTML', period: '1年' },
            { name: 'CSS', period: '1年' },
            { name: 'Javascript', period: '1年' },
          ],
        },
        backend: {
          title: 'バックエンド',
          fields: [
            { key: 'name', label: '技術' },
            { key: 'period', label: '経験年数' },
          ],
          skills: [
            { name: 'PHP', period: '1年' },
            { name: 'Ruby', period: '3年' },
            { name: 'VB6', period: '3年' },
            { name: 'Perl', period: '3年' },
          ],
        },
        other: {
          title: 'その他',
          fields: [
            { key: 'name', label: '技術' },
            { key: 'period', label: '経験年数' },
          ],
          skills: [{ name: 'Emacs', period: '4年' }],
        },
      },
    }
  },
}
</script>

<style lang="sass" scoped>
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@300;500;700&display=swap');

.main-container-outer
  font-family: 'Noto Sans JP'
  background-color: #fafafa
.main-container-inner
  width: 80%
  margin: 0 auto
</style>
