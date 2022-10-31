<template>
    <div class="single form-group">
        <label for class="font-size-sm font-weight-bold text-primary">
            {{label}}
        </label>
        <input type="file" ref="uploadInput" @change="handleChange()" class="form-control upload-input" />
        <div class="uploader-mask d-flex justify-content-center align-items-center">
            <!--Upload de arquivo ícones criados por Pavani TLN - https://www.flaticon.com/br/icones-gratis/upload-de-arquivo-->
            <img src="@/assets/upload.png" class="uploader-icon img-fluid" alt />
        </div>
    </div>
</template>

<script>
export default {
    props: {
        label: {
            type: String,
            required: false,
            default: "Upload um arquivo",
        },
    },

    methods: {
        handleChange() {
            console.log(this.$refs.uploadInput.files);
        }
    }
};
</script>