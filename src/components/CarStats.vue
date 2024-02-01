<script setup></script>

<template>
  <div class="container-fluid mt-2">
    <div class="row justify-content-center">
      <div class="col-9">
        <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
          <div class="carousel-indicators">
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              data-bs-slide-to="0"
              class="active"
              aria-current="true"
              aria-label="Slide 1"
            ></button>
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              data-bs-slide-to="1"
              aria-label="Slide 2"
            ></button>
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              data-bs-slide-to="2"
              aria-label="Slide 3"
            ></button>
          </div>
          <div class="carousel-inner">
            <div class="carousel-item sizing-container active">
              <img
                src="../assets/images/see-through.png"
                class="d-block w-100 sizing"
                alt="..."
                style="object-fit: cover"
              />
              <div class="carousel-caption d-none d-md-block transparent-bg mid-right-text">
                <h5>Engine</h5>
                <!-- <p>Some representative placeholder content for the first slide.</p> -->
                <table>
                  <tbody>
                    <!-- <tr>
                      <td id="Engine" style="text-align: left" colspan="2"></td>
                    </tr> -->
                    <tr>
                      <td>Configuration</td>
                      <td>Straight 5</td>
                    </tr>
                    <tr>
                      <td>Location</td>
                      <td>Front, longitudinally-mounted</td>
                    </tr>
                    <tr>
                      <td>Construction</td>
                      <td>Aluminum alloy block and head</td>
                    </tr>
                    <tr>
                      <td>Displacement</td>
                      <td>2,110 cc / 128.8 cu in</td>
                    </tr>
                    <tr>
                      <td>Bore / Stroke</td>
                      <td>79.5 mm (3.1 in) / 85.0 mm (3.3 in)</td>
                    </tr>
                    <tr>
                      <td>Compression</td>
                      <td>7.5:1</td>
                    </tr>
                    <tr>
                      <td>Valvetrain</td>
                      <td>4 valves / cylinder, DOHC</td>
                    </tr>
                    <tr>
                      <td>Fuel feed</td>
                      <td>Fuel Injection</td>
                    </tr>
                    <tr>
                      <td>Lubrication</td>
                      <td>Dry sump</td>
                    </tr>
                    <tr>
                      <td>Aspiration</td>
                      <td>KKK Turbo</td>
                    </tr>
                    <tr>
                      <td>Power</td>
                      <td>540 bhp / 403 kW @ 7,500 rpm</td>
                    </tr>
                    <tr>
                      <td>Torque</td>
                      <td>590 Nm / 435 ft-lbs @ 5,500 rpm</td>
                    </tr>
                    <tr>
                      <td>BHP/Liter</td>
                      <td>256 bhp / liter</td>
                    </tr>
                  </tbody>
                </table>
              </div>
            </div>
            <div class="carousel-item sizing-container">
              <img
                src="../assets/images/head-on.png"
                class="d-block w-100 sizing"
                alt="..."
                style="object-fit: cover"
              />
              <div class="carousel-caption d-none d-md-block transparent-bg mid-right-text">
                <h5>Drivetrain</h5>
                <!-- <p>Some representative placeholder content for the second slide.</p> -->
                <table>
                  <tbody>
                    <!-- <tr>
                      <td id="Drivetrain" colspan="2"></td>
                    </tr> -->
                    <tr>
                      <td>Chassis</td>
                      <td>kevlar body on steel monocoque</td>
                    </tr>
                    <tr>
                      <td>Suspension (fr/r)</td>
                      <td>McPherson struts, coil springs, &amp; shock absorbers</td>
                    </tr>
                    <tr>
                      <td>Steering</td>
                      <td>rack-and-pinion, power-assisted</td>
                    </tr>
                    <tr>
                      <td>Brakes</td>
                      <td>ventilated discs, all-round</td>
                    </tr>
                    <tr>
                      <td>Gearbox</td>
                      <td>6-speed Sequential</td>
                    </tr>
                    <tr>
                      <td>Clutch</td>
                      <td>Dry, single plate</td>
                    </tr>
                    <tr>
                      <td>Drive</td>
                      <td>Quattro All wheel drive</td>
                    </tr>
                  </tbody>
                </table>
              </div>
            </div>
            <div class="carousel-item sizing-container">
              <img
                src="../assets/images/stripped-down.jpg"
                class="d-block w-100 sizing"
                alt="..."
                style="transform: scale(-1, -1)"
              />
              <div class="carousel-caption d-none d-md-block transparent-bg mid-right-text">
                <h5>Dimensions</h5>
                <!-- <p>Some representative placeholder content for the third slide.</p> -->
                <table>
                  <tbody>
                    <!-- <tr>
                      <td id="Dimensions" colspan="2"></td>
                    </tr> -->
                    <tr>
                      <td>Weight</td>
                      <td>1,090 kilo / 2,403 lbs</td>
                    </tr>
                    <tr>
                      <td>Length / Width / Height</td>
                      <td>4,240 mm (166.9 in) / 1,860 mm (73.2 in) / 1,344 mm (52.9 in)</td>
                    </tr>
                    <tr>
                      <td>Wheelbase / Track (fr/r)</td>
                      <td>2,224 mm (87.6 in) / 1,465 mm (57.7 in) / 1,502 mm (59.1 in)</td>
                    </tr>
                    <tr>
                      <td>Fuel tank</td>
                      <td>120 Litre (31.7 Gallon US / 26.4 Gallon Imperial)</td>
                    </tr>
                    <tr>
                      <td>Wheels</td>
                      <td>9J x 16</td>
                    </tr>
                    <tr>
                      <td>Tires</td>
                      <td>18/68 – 16</td>
                    </tr>
                  </tbody>
                </table>
              </div>
            </div>
          </div>
          <!-- <button
            class="carousel-control-prev"
            type="button"
            data-bs-target="#carouselExampleCaptions"
            data-bs-slide="prev"
          >
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
          </button>
          <button
            class="carousel-control-next"
            type="button"
            data-bs-target="#carouselExampleCaptions"
            data-bs-slide="next"
          >
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
          </button> -->
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.sizing {
  object-fit: cover;
  width: 100%;
  height: 100%;
}

.sizing-container {
  height: 50rem;
  position: relative;
}

.transparent-bg {
  background-color: rgba(0, 0, 0, 0.6);
  border-radius: 10px;
  color: #ffc11c;
}

.mid-right-text {
  position: absolute;
  top: 5%;
  right: 1%;
  left: 70%;
  bottom: 5%;
}

table {
  width: 100%;
  margin-bottom: 30px;
  display: table;
  border-collapse: separate;
  box-sizing: border-box;
  text-indent: initial;
  border-spacing: 2px;
  border-color: #ffc11c;
  padding: 10px;
}
tr {
  display: table-row;
  vertical-align: inherit;
  border-color: inherit;
}
table td,
table th {
  border-top: 1px solid #ffc11c;
  padding: 10px 5px;
}
</style>
