<template>
    <div class="slider">
      <div class="slide-track">
        <div class="slide">
          <img src="https://www.ufpe.br/image/company_logo?img_id=20911&t=1662385233867" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="https://yata-apix-156beb63-a777-4ad4-b514-b097223d5325.s3-object.locaweb.com.br/59177deedeea491c92ebad34c8ecc0a9.png" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="https://www.ufpe.br/image/company_logo?img_id=20911&t=1662385233867" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="https://seeklogo.com/images/E/ete-logo-C00FB6F54C-seeklogo.com.png" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="https://www.ufpe.br/image/company_logo?img_id=20911&t=1662385233867" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="http://www1.unicap.br/cbs/wp-content/uploads/2019/05/Logo-unicap.png" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="https://yata-apix-156beb63-a777-4ad4-b514-b097223d5325.s3-object.locaweb.com.br/59177deedeea491c92ebad34c8ecc0a9.png" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="https://www.ufpe.br/image/company_logo?img_id=20911&t=1662385233867" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="https://yata-apix-156beb63-a777-4ad4-b514-b097223d5325.s3-object.locaweb.com.br/59177deedeea491c92ebad34c8ecc0a9.png" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="https://images.educamaisbrasil.com.br/content/tecnico/instituicao/logo/g/unifg-centro-universitario-dos-guararapes.png" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="https://seeklogo.com/images/E/ete-logo-C00FB6F54C-seeklogo.com.png" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/557257/5.png" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="http://www1.unicap.br/cbs/wp-content/uploads/2019/05/Logo-unicap.png" height="100" width="250" alt="" />
        </div>
        <div class="slide">
          <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/557257/7.png" height="100" width="250" alt="" />
        </div>
      </div>
    </div>
</template>

<script>
    export default {
      name:"Carrossel"
    }
</script>

<style scoped>

@keyframes scroll {
	0% { transform: translateX(0); }
	100% { transform: translateX(calc(-250px * 7))}
}

.slider {
	background: #125c12;
	box-shadow: 0 10px 20px -5px rgba(0, 0, 0, .125);
	height: 100px;
	margin: auto;
	overflow:hidden;
	position: relative;
	width: 100%;
}

.slider::before, .slider::after {
		content: "";
		height: 100px;
		position: absolute;
		width: 200px;
		z-index: 2;
}
	
.slider::after {
		right: 0;
		top: 0;
		transform: rotateZ(180deg);
}

.slider::before {
		left: 0;
		top: 0;
}
	
.slide-track {
		animation: scroll 40s linear infinite;
		display: flex;
		width: calc(250px * 14);
}
	
.slide {
		height: 100px;
		width: 250px;
}

</style>