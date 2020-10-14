<script>
import CreateBlog from '~/pages/blog/create'

export default {
  name: 'Id',
  extends: CreateBlog,
  fetch() {
    this.loadImageInfo()
  },
  methods: {
    async loadImageInfo() {
      const id = this.$route.params.id
      this.model = await this.$axios.$get(`https://picsum.photos/id/${id}/info`)
    },
  },
}
</script>
