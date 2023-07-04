<template>
  <div class="profile">
    <b-breadcrumb :items="breadcrumb" />
    <ProfileForm />
  </div>
</template>

<script>
import ProfileForm from '@/components/admin/ProfileForm'
export default {
  layout: 'admin',
  components: {
    ProfileForm
  },
  data () {
    return {
      breadcrumb: [
        { text: 'Painel', to: '/admin' },
        { text: 'Perfil do usuário', active: true }
      ]
    }
  }
}
</script>
