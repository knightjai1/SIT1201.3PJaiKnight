<template>
    <div>
        <button @click="downloadFile">Download File</button>
    </div>
</template>

<script>
export default {
    methods: {
        downloadFile() {
            const filePath = '../cv.pdf';

            const link = document.createElement('a');
            link.href = filePath;
            link.setAttribute('download', 'MyCV.pdf');
            link.style.display = 'none';

            document.body.appendChild(link);
            link.click();

            document.body.removeChild(link);
        },
    },
};
</script>