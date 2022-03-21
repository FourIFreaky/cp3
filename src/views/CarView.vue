<template>
    <div>
        <div class="pure-menu pure-menu-horizontal">
            <ul class="pure-menu-list">
                <li class="pure-menu-item"><a @click="clearAll()" href="#" class="pure-menu-link">Clear All</a></li>
                <li class="pure-menu-item"><a @click="clearMake()" href="#" class="pure-menu-link">Clear Make</a></li>
                <li class="pure-menu-item"><a @click="clearModel()" href="#" class="pure-menu-link">Clear Model</a></li>
                <li class="pure-menu-item"><a @click="clearYear()" href="#" class="pure-menu-link">Clear Year</a></li>
                <li class="pure-menu-item pure-menu-has-children pure-menu-allow-hover"><a href="#" class="pure-menu-link">Make</a>
                    <ul class="pure-menu-children">
                        <li class="pure-menu-item"><a @click="selectMake('Nissan')" href="#" class="pure-menu-link">Nissan</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Ford')" href="#" class="pure-menu-link">Ford</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Kia')" href="#" class="pure-menu-link">Kia</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Mazda')" href="#" class="pure-menu-link">Mazda</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Lincoln')" href="#" class="pure-menu-link">Lincoln</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Hyundai')" href="#" class="pure-menu-link">Hyundai</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Volvo')" href="#" class="pure-menu-link">Volvo</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Lexus')" href="#" class="pure-menu-link">Lexus</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Chevrolet')" href="#" class="pure-menu-link">Chevrolet</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Porsche')" href="#" class="pure-menu-link">Porsche</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Subaru')" href="#" class="pure-menu-link">Subaru</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Maybach')" href="#" class="pure-menu-link">Maybach</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Acura')" href="#" class="pure-menu-link">Acura</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Mercedes-Benz')" href="#" class="pure-menu-link">Mercedes-Benz</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Pontiac')" href="#" class="pure-menu-link">Pontiac</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Land Rover')" href="#" class="pure-menu-link">Land Rover</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('BMW')" href="#" class="pure-menu-link">BMW</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Saab')" href="#" class="pure-menu-link">Saab</a></li>
                        <li class="pure-menu-item"><a @click="selectMake('Audi')" href="#" class="pure-menu-link">Audi</a></li>
                    </ul>
                </li>
                <li class="pure-menu-item pure-menu-has-children pure-menu-allow-hover"><a href="#" class="pure-menu-link">Model</a>
                    <ul class="pure-menu-children">
                        <li class="pure-menu-item"><a @click="selectModel('Altima')" href="#" class="pure-menu-link">Altima</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Tempo')" href="#" class="pure-menu-link">Tempo</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Sportage')" href="#" class="pure-menu-link">Sportage</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('626')" href="#" class="pure-menu-link">626</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Town Car')" href="#" class="pure-menu-link">Town Car</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Sonata')" href="#" class="pure-menu-link">Sonata</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Econoline E250')" href="#" class="pure-menu-link">Econoline E250</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('C70')" href="#" class="pure-menu-link">C70</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('LX')" href="#" class="pure-menu-link">LX</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Suburban')" href="#" class="pure-menu-link">Suburban</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Mustang')" href="#" class="pure-menu-link">Mustang</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Express 150')" href="#" class="pure-menu-link">Express 1500</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Boxster')" href="#" class="pure-menu-link">Boxster</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Legacy')" href="#" class="pure-menu-link">Legacy</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('57')" href="#" class="pure-menu-link">57</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Legend')" href="#" class="pure-menu-link">Legend</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('A7')" href="#" class="pure-menu-link">A7</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('E-Class')" href="#" class="pure-menu-link">E-Class</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('G-Class')" href="#" class="pure-menu-link">G-Class</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Grand Prix')" href="#" class="pure-menu-link">Grand Prix</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Navigator L')" href="#" class="pure-menu-link">Navigator L</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('Defender')" href="#" class="pure-menu-link">Defender</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('7-Series')" href="#" class="pure-menu-link">7 Series</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('LTD Crown Victoria')" href="#" class="pure-menu-link">LTD Crown Victoria</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('900')" href="#" class="pure-menu-link">900</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('A8')" href="#" class="pure-menu-link">A8</a></li>
                        <li class="pure-menu-item"><a @click="selectModel('LeMans')" href="#" class="pure-menu-link">LeMans</a></li>
                    </ul>
                </li>
                <li class="pure-menu-item pure-menu-has-children pure-menu-allow-hover"><a href="#" class="pure-menu-link">Year</a>
                    <ul class="pure-menu-children">
                        <li class="pure-menu-item"><a @click="selectDecade(0)" href="#" class="pure-menu-link">1980-1989</a></li>
                        <li class="pure-menu-item"><a @click="selectDecade(1)" href="#" class="pure-menu-link">1900-1999</a></li>
                        <li class="pure-menu-item"><a @click="selectDecade(2)" href="#" class="pure-menu-link">2000-2009</a></li>
                        <li class="pure-menu-item"><a @click="selectDecade(3)" href="#" class="pure-menu-link">2010-2019</a></li>
                    </ul>
                </li>
            </ul>
        </div>
        <CarList :cars="cars"/>
    </div>
</template>

<script>
    import CarList from "../components/CarList.vue"
    export default {
        name: 'theCars',
        components: {
            CarList
        },
        data() {
            return {
                car_make: '',
                car_model: '',
                car_model_year: '',
                decade: '',
            }
        },
        computed: {
            cars() {
                return this.$root.$data.cars.filter(car => ((this.car_make === car.car_make) && (this.car_model === '') && (this.decade === '')) ||
                                                            ((this.car_model === car.car_model) && (this.car_make === '') && (this.decade === '')) ||
                                                            ((this.car_make === '') && (this.car_model === '') && (this.decade === car.decade)) ||
                                                            ((car.car_make === this.car_make) && (car.car_model === this.car_model) && (this.decade === '')) ||
                                                            ((this.car_make === car.car_make) && (this.car_model === '') && (this.decade === car.decade)) ||
                                                            ((this.car_make === '') && (this.car_model === car.car_model) && (this.decade === car.decade)) ||
                                                            ((this.car_make === car.car_make) && (this.car_model === car.car_model) && (this.decade === car.decade)));
            }
        },
        methods: {
            clearAll() {
                this.car_make = '';
                this.car_model = '';
                this.car_model_year = '';
            },
            clearMake() {
                this.car_make = '';
            },
            clearModel() {
                this.car_model = '';
            },
            clearyear() {
                this.car_model_year = '';
            },
            selectMake(car_make) {
                this.car_make = car_make;
            },
            selectModel(car_model) {
                this.car_model = car_model;
            },
            selectDecade(decade) {
                this.decade = decade;
            }
            
        }
    }
</script>