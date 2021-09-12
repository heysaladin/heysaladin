---
layout: home
title: "Contact"
---

<section id="opening" class="h-100 w-100 bg-white" style="box-sizing: border-box; ">
<div class="container-xxl mx-auto p-0  position-relative header-2-1" style="font-family: 'Poppins', sans-serif">
        <div>
            <div class="mx-auto d-flex flex-lg-column flex-column hero">

    <h4>Send me a message</h4>

    <form id="contactform" name="contactform" onsubmit="return validateForm()" method="POST">
    <div class="form-group">
        <div class="input-group">
        <span class="input-group-addon">Name</span>
        <input type="text" name="name" class="form-control" required>
        </div>
        <div class="input-group">
        <span class="input-group-addon">Email</span>
        <input type="email" name="_replyto" class="form-control" required>
        </div>
        <div class="input-group">
        <span class="input-group-addon">Subject</span>
        <input type="text" name="subject" class="form-control" required>
        </div>
        <div class="input-group">
        <span class="input-group-addon">Description</span>
        <textarea name="description" class="form-control" rows="4" cols="60" required></textarea>
        </div>
        <input type="hidden" name="project_type" value="UI/UX Design" />
        <input type="hidden" name="team" value="HeySaladin" />
        <input type="hidden" name="come_from" value="https://heysaladin.com/" />
        <!-- <input type="text" name="_gotcha" style="display:none" /> -->
        <button name="submit" type="submit" id="sendMessage">Send</button>
    </div>
    </form>

                </div>
            </div>
        </div>

</section>
<section id="action" class="h-100 w-100 bg-white" style="box-sizing: border-box; ">
<div class="container-xxl mx-auto p-0  position-relative header-2-1" style="font-family: 'Poppins', sans-serif">
        <div>
            <div class="mx-auto d-flex flex-lg-column flex-column hero">
    <h4>or send an Email directly</h4>
    <button onclick="location.href='mailto:heysaladin@gmail.com';"
    style="margin:24px auto 0;background-color:white;border:solid 1px #8254e5;color:#8254e5;height:50px;padding:16px 32px;font-family:Montserrat,sans-serif;font-weight:700;font-size:.688rem;line-height:18px;letter-spacing:1.54px;text-transform:uppercase;border-radius:25px;">Email
    me!</button>
                </div>
            </div>
        </div>
</section>

<style>
    section h4 {
        text-align: center;
        font-size: 22pt;
        font-weight: bold;
        margin-bottom: 1rem;
    }
    .input-group {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: flex-start;
    flex-direction: column;
    margin: 14px 0;
    }
    .input-group span {
        display: block;
        margin: 0 0 6px 0;
    }
    .input-group input {
        display: block;
        width: 100%;
        height: 32px;
    }
    input, textarea {
        width: 100% !important;
        border-radius: 6px;
        border: solid 1px grey;
    }
    form button {
        border: none;
        font-weight: bold;
        text-transform: uppercase;
        color: #fff;
        background-image: linear-gradient(135deg, #8254e5, #83afe3 150%);
        padding: 14px 36px;
        border-radius: 24px;
        margin-top: 20px;
        box-shadow: 0 11px 36px 0 rgb(70 89 138 / 25%);
        font-weight: 700;
        letter-spacing: 1.54px;
    }
</style>

<!-- <section class="h-100 w-100 bg-white" style="box-sizing: border-box; ">
    <div class="container-xxl mx-auto p-0  position-relative header-2-1" style="font-family: 'Poppins', sans-serif">
        <div>
            <div class="mx-auto d-flex flex-lg-row flex-column hero">
                <div class="left-column d-flex flex-lg-grow-1 flex-column align-items-lg-start text-lg-start align-items-center text-center"
                    id="hero-text">
                    <h1 class="">
                        Contact
                    </h1>
                </div>
            </div>
        </div>
    </div>
</section> -->

  <script src="https://code.jquery.com/jquery-3.5.1.min.js"
    integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0=" crossorigin="anonymous"></script>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/sweetalert/2.1.2/sweetalert.min.js"
    integrity="sha512-AA1Bzp5Q0K1KanKKmvN/4d3IRKVlv9PYgwFPvm32nPO6QS8yH1HO7LbgB1pgiOxPtfeg5zEn2ba64MUcqJx6CA=="
    crossorigin="anonymous"></script>

  <script>
    var message = "";
    var url = "";
    var xhr = "";

    var name = "";
    var email_address = "";
    var project_type = "";

    function validateEmail(email) {
      var re =
        /^(?:[a-z0-9!#$%&amp;'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&amp;'*+/=?^_`{|}~-]+)*|"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\])$/;
      return re.test(email);
    }

    $("#sendMessage").on("click", function (e) {
      e.preventDefault();

      name = document.forms["contactform"]["name"].value;
      email_address = document.forms["contactform"]["_replyto"].value;
      phone_number = '0';
      subject = document.forms["contactform"]["subject"].value;
      description = document.forms["contactform"]["description"].value;
      project_type = document.forms["contactform"]["project_type"].value;
      team = document.forms["contactform"]["team"].value;
      come_from = document.forms["contactform"]["come_from"].value;

      message = $("#contactform").serialize();

      url =
        'https://script.google.com/macros/s/AKfycbzIP5lx22SmZKerNk_siXwZmT8BzpEKNgQzd618IPZCJY1L2LZ6dnj1bA/exec?name=' +
        document.forms["contactform"]["name"].value + '&' +
        'email_address=' + document.forms["contactform"]["_replyto"].value + '&' +
        'phone_number=' + phone_number + '&' +
        'project_type=' + document.forms["contactform"]["project_type"].value + '&' +
        'team=' + document.forms["contactform"]["team"].value + '&' +
        'come_from=' + document.forms["contactform"]["come_from"].value + '&' +
        'subject=' + document.forms["contactform"]["subject"].value + '&' +
        'description=' + document.forms["contactform"]["description"].value;

      if (name == "") {
        swal("Oh no...", "Please tell us your name!", "error", {
          button: "OK!",
        });
        return false;
      } else if (name.length < 6) {
        swal("Oh please...", "Your name must more than 5 characters!", "error", {
          button: "OK!",
        });
        return false;
      } else if (email_address == "") {
        swal("Please...", "Please tell us your email!", "error", {
          button: "OK!",
        });
        return false;
      } else if (validateEmail(email_address) == false) {
        swal("Please fix it!", "You have entered an invalid email address.", "error", {
          button: "OK!",
        });
        return false;
      } else if (subject == "") {
        swal("Oh no...", "Please tell us your subject!", "error", {
          button: "OK!",
        });
        return false;
      } else if (subject.length < 6) {
        swal("Oh please...", "Your subject must more than 5 characters!", "error", {
          button: "OK!",
        });
        return false;
      } else if (description == "") {
        swal("Oh no...", "Please tell us your description!", "error", {
          button: "OK!",
        });
        return false;
      } else if (description.length < 6) {
        swal("Oh please...", "Your description must more than 5 characters!", "error", {
          button: "OK!",
        });
        return false;
      }
      /* else if (phone_number == "") {
        swal("Please...", "Please tell us your phone number!", "error", {
          button: "OK!",
        });
        return false;
      } else if (typeof parseInt(phone_number) != 'number') {
        swal("Oops...", "Phone number must number!", "error", {
          button: "OK!",
        });
        return false;
      } else if (phone_number.length < 10) {
        swal("Oh please...", "Your phone number length must more than 9!", "error", {
          button: "OK!",
        });
        return false;
      } */
      else if (project_type == "default") {
        swal("Cool, but...", "Please select the project type!", "error", {
          button: "OK!",
        });
        return false;
      } else {

        // console.log(url);

        xhr = new XMLHttpRequest();
        xhr.open('GET', url);
        xhr.onload = function () {
          if (xhr.status === 200) {
            $.ajax({
              url: "https://formspree.io/f/mrgovjjw",
              method: "POST",
              data: {
                message: message
              },
              dataType: "json"
            });

            setTimeout(function () {
              swal("Succeed!", "Your message has been sent!", "success", {
                  button: "OK!",
                })
                .then(() => {
                  window.location = "index.html";
                });
            }, 300);

            /*
            setTimeout(function () {
              swal({
                title: "Yeeey!",
                text: "Your message has been successfully sent!",
                type: "success"
                // }, function() {
                //     window.location = './index.html';
              }).then(function () {
                window.location = './index.html';
              });
            }, 600);
            */

          } else {
            swal("Sorry...", "Error server, try again later!", "error", {
              button: "OK!",
            });
          }
        };
        xhr.send();

      }
      return false;

    });
  </script>

  <script>
    function myFunction() {
      var x = document.getElementById("myTopnav");
      if (x.className === "topnav") {
        x.className += " responsive";
      } else {
        x.className = "topnav";
      }
    }
  </script>
