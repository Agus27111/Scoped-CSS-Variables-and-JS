I have try 3 times

#first one just like the tutorial (i look pause and try)

//grab All inputs in class controls
const inputs = document.querySelectorAll(".controls input");

      function changeControl() {
        //get the international units for the value
        const suffix = this.dataset.sizing || ""; //mengambil sizing 'px' yang sudah di declare di HTML
        document.documentElement.style.setProperty(
          `--${this.name}`,
          this.value + suffix
        );
      }

      // untuk mendeteksi setiap gerakan dengan eventlistener
      inputs.forEach((input) =>
        input.addEventListener("change", changeControl)
      );
      inputs.forEach((input) =>
        input.addEventListener("mousemove", changeControl)
      );

#second time i dont see the tutorial and i just try and search google and chatGPT

i will try again my code
grap All inputs
const inputs = document.querySelectorAll(".controls input");

      function changeValue() {
        //memasukkan style ke element pakai JS
        // document.documentElement.style.setProperty(
        //   `--${this.name}`,
        //   this.value + "px"
        // ); i have try this its Work but not for the color
        const units = this.dataset.sizing || "";
        document.documentElement.style.setProperty(
          `--${this.name}`,
          this.value + units
        );
      }

      //add eventlistener for add some value
      inputs.forEach((input) => {
        input.addEventListener("change", changeValue);
      });
      inputs.forEach((input) => {
        input.addEventListener("mousemove", changeValue);
      });

    #Third i just improve my Code for the posibilty, and thats my code in HTML structure
