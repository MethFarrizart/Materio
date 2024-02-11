<template>
    <v-container style="background-color: rgba(30, 143, 255, 0.313)">
        <v-row>
            <v-col cols="3">
                <v-card style="height: 12rem">
                    <v-card-title
                        >Congratulations John!
                        <v-icon class="ps-3" color="warning">
                            mdi-robot-happy-outline</v-icon
                        >
                    </v-card-title>
                    <v-card-text>You have won Trophy</v-card-text>

                    <v-row>
                        <v-col cols="6">
                            <v-card-text
                                class="text-primary font-weight-bold text-h5"
                                >$42.8k</v-card-text
                            >
                            <v-card-text class="mt-n4">
                                <v-btn color="primary">View Sales</v-btn>
                            </v-card-text>
                        </v-col>
                        <v-col cols="6">
                            <v-img
                                class="w-100 h-100 mt-n11"
                                src="https://media.istockphoto.com/id/1168757141/vector/gold-trophy-with-the-name-plate-of-the-winner-of-the-competition.jpg?s=612x612&w=0&k=20&c=ljsP4p0yuJnh4f5jE2VwXfjs96CC0x4zj8CHUoMo39E="
                            ></v-img>
                        </v-col>
                    </v-row>
                </v-card>
            </v-col>

            <v-col cols="9">
                <v-card style="height: 12rem">
                    <v-row>
                        <v-col cols="6">
                            <v-card-title>Statistics Card </v-card-title>
                            <v-card-text
                                >Total 48.5% Growth &#128526; this
                                month</v-card-text
                            >
                        </v-col>
                        <v-col cols="6" align="right">
                            <div class="mt-5">
                                <v-icon>mdi-dots-vertical</v-icon>
                            </div>
                        </v-col>
                    </v-row>

                    <v-row>
                        <v-col cols="3">
                            <div class="d-flex ps-4" style="gap: 15px">
                                <v-card class="pa-3 bg-primary">
                                    <v-icon>mdi-trending-up</v-icon>
                                </v-card>
                                <div class="d-flex flex-column">
                                    <div class="text-caption grey-lighten-5">
                                        Sales
                                    </div>
                                    <div
                                        class="text-subtitle-1 font-weight-bold"
                                    >
                                        245k
                                    </div>
                                </div>
                            </div>
                        </v-col>

                        <v-col cols="3">
                            <div class="d-flex ps-4" style="gap: 15px">
                                <v-card class="pa-3 bg-success">
                                    <v-icon>mdi-account-outline</v-icon>
                                </v-card>
                                <div class="d-flex flex-column">
                                    <div class="text-caption grey-lighten-5">
                                        Customers
                                    </div>
                                    <div
                                        class="text-subtitle-1 font-weight-bold"
                                    >
                                        12.5k
                                    </div>
                                </div>
                            </div>
                        </v-col>

                        <v-col cols="3">
                            <div class="d-flex ps-4" style="gap: 15px">
                                <v-card class="pa-3 bg-warning">
                                    <v-icon>mdi-package-variant-closed</v-icon>
                                </v-card>
                                <div class="d-flex flex-column">
                                    <div class="text-caption grey-lighten-5">
                                        Product
                                    </div>
                                    <div
                                        class="text-subtitle-1 font-weight-bold"
                                    >
                                        1.54k
                                    </div>
                                </div>
                            </div>
                        </v-col>

                        <v-col cols="3">
                            <div class="d-flex ps-4" style="gap: 15px">
                                <v-card class="pa-3 bg-info">
                                    <v-icon>mdi-currency-usd</v-icon>
                                </v-card>
                                <div class="d-flex flex-column">
                                    <div class="text-caption grey-lighten-5">
                                        Revenue
                                    </div>
                                    <div
                                        class="text-subtitle-1 font-weight-bold"
                                    >
                                        $88k
                                    </div>
                                </div>
                            </div>
                        </v-col>
                    </v-row>
                </v-card>
            </v-col>
        </v-row>

        <v-row class="mt-8">
            <v-col cols="3">
                <v-card class="pb-4">
                    <v-row>
                        <v-col cols="6">
                            <v-card-title>Weekly Overview </v-card-title>
                        </v-col>
                        <v-col cols="6" align="right">
                            <div class="mt-3">
                                <v-icon>mdi-dots-vertical</v-icon>
                            </div>
                        </v-col>
                    </v-row>

                    <v-row>
                        <v-col cols="12">
                            <v-card-text class="mt-n5"
                                ><Bar :data="chartData"
                            /></v-card-text>
                        </v-col>

                        <v-col cols="3">
                            <div class="d-flex">
                                <v-card-title class="text-h5 font-weight-bold">
                                    45%</v-card-title
                                >
                            </div>
                        </v-col>

                        <v-col cols="7">
                            <div class="text-subtitle-2 grey-lighten-5">
                                Your sales performance in 45% &#128525; better
                                compare to last month
                            </div>
                        </v-col>
                    </v-row>
                    <div align="center">
                        <v-btn
                            class="w-75 font-weight-bold mt-5"
                            variant="outlined"
                            color="primary"
                            style="border-color: blueviolet"
                        >
                            Details</v-btn
                        >
                    </div>
                </v-card>
            </v-col>

            <v-col cols="9">
                <v-row>
                    <v-col cols="6">
                        <v-card class="pb-10">
                            <v-row>
                                <v-col cols="6">
                                    <v-card-title>Total Earning</v-card-title>
                                </v-col>
                                <v-col cols="6" align="right">
                                    <div class="mt-3">
                                        <v-icon>mdi-dots-vertical</v-icon>
                                    </div>
                                </v-col>
                            </v-row>

                            <v-card-text>
                                <div class="d-flex">
                                    <div class="text-h4 font-weight-bold">
                                        $24,895
                                    </div>
                                    <div class="text-h5 text-success pt-1">
                                        <v-icon>mdi-menu-up</v-icon
                                        ><small>10%</small>
                                    </div>
                                </div>

                                <div class="pt-4">
                                    Compared to $84,325 last year
                                </div>
                            </v-card-text>

                            <v-row class="mt-5">
                                <v-col cols="12">
                                    <div class="d-flex justify-space-between">
                                        <div
                                            class="d-flex ps-4"
                                            style="gap: 15px"
                                        >
                                            <v-card
                                                class="pa-3 bg-grey-lighten-5"
                                            >
                                                <v-icon
                                                    color="light-blue-darken-2"
                                                    >mdi-triangle</v-icon
                                                >
                                            </v-card>
                                            <div class="d-flex flex-column">
                                                <div
                                                    class="text-subtitle-1 font-weight-bold"
                                                >
                                                    Zipcar
                                                </div>
                                                <div
                                                    class="text-caption grey-lighten-5"
                                                >
                                                    Vuejs, React & HTML
                                                </div>
                                            </div>
                                        </div>

                                        <div class="d-flex flex-column mx-4">
                                            <div
                                                class="text-subtitle-1 font-weight-bold"
                                            >
                                                $24,895.65
                                            </div>
                                            <v-progress-linear
                                                model-value="85"
                                                color="primary"
                                            ></v-progress-linear>
                                        </div>
                                    </div>
                                </v-col>

                                <v-col cols="12">
                                    <div class="d-flex justify-space-between">
                                        <div
                                            class="d-flex ps-4"
                                            style="gap: 15px"
                                        >
                                            <v-card
                                                class="pa-3 bg-grey-lighten-5"
                                            >
                                                <v-icon color="orange-darken-1"
                                                    >mdi-flash</v-icon
                                                >
                                            </v-card>
                                            <div class="d-flex flex-column">
                                                <div
                                                    class="text-subtitle-1 font-weight-bold"
                                                >
                                                    Bitbank
                                                </div>
                                                <div
                                                    class="text-caption grey-lighten-5"
                                                >
                                                    Sketch, Figma and XD
                                                </div>
                                            </div>
                                        </div>

                                        <div class="d-flex flex-column mx-4">
                                            <div
                                                class="text-subtitle-1 font-weight-bold"
                                            >
                                                $86500.20
                                            </div>
                                            <v-progress-linear
                                                model-value="65"
                                                color="info"
                                            ></v-progress-linear>
                                        </div>
                                    </div>
                                </v-col>

                                <v-col cols="12">
                                    <div class="d-flex justify-space-between">
                                        <div
                                            class="d-flex ps-4"
                                            style="gap: 15px"
                                        >
                                            <v-card
                                                class="pa-3 bg-grey-lighten-5"
                                            >
                                                <v-icon
                                                    color="light-blue-accent-4"
                                                    >mdi-react</v-icon
                                                >
                                            </v-card>
                                            <div class="d-flex flex-column">
                                                <div
                                                    class="text-subtitle-1 font-weight-bold"
                                                >
                                                    Aviato
                                                </div>
                                                <div
                                                    class="text-caption grey-lighten-5"
                                                >
                                                    HTML & Angular
                                                </div>
                                            </div>
                                        </div>

                                        <div class="d-flex flex-column mx-4">
                                            <div
                                                class="text-subtitle-1 font-weight-bold"
                                            >
                                                $12450.80
                                            </div>
                                            <v-progress-linear
                                                model-value="30"
                                                color="grey"
                                            ></v-progress-linear>
                                        </div>
                                    </div>
                                </v-col>
                            </v-row>
                        </v-card>
                    </v-col>

                    <v-col cols="6">
                        <v-row>
                            <v-col cols="6">
                                <v-card class="pb-1">
                                    <v-row>
                                        <v-col cols="6">
                                            <v-card-title>
                                                <div
                                                    class="bg-success text-center pt-1"
                                                    style="
                                                        border-radius: 50%;
                                                        width: 40px;
                                                        height: 40px;
                                                        font-size: 15px;
                                                    "
                                                >
                                                    <v-icon>mdi-poll</v-icon>
                                                </div>
                                            </v-card-title>
                                        </v-col>
                                        <v-col cols="6" align="right">
                                            <div class="mt-3">
                                                <v-icon
                                                    >mdi-dots-vertical</v-icon
                                                >
                                            </div>
                                        </v-col>
                                    </v-row>

                                    <v-card-text>
                                        <div
                                            class="text-body font-weight-bold mt-1"
                                        >
                                            Total Profit
                                        </div>
                                        <div class="d-flex mt-3">
                                            <div
                                                class="text-h5 font-weight-bold"
                                            >
                                                $25.6k
                                            </div>
                                            <div
                                                class="text-body-1 font-size-3 text-success mx-2 pt-1"
                                            >
                                                +<small>42%</small>
                                            </div>
                                        </div>

                                        <div class="pt-4">Weekly Project</div>
                                    </v-card-text>
                                </v-card>
                            </v-col>

                            <v-col cols="6">
                                <v-card class="pb-1">
                                    <v-row>
                                        <v-col cols="6">
                                            <v-card-title>
                                                <div
                                                    class="bg-grey-darken-2 text-center pt-1"
                                                    style="
                                                        border-radius: 50%;
                                                        width: 40px;
                                                        height: 40px;
                                                        font-size: 15px;
                                                    "
                                                >
                                                    <v-icon
                                                        >mdi-currency-usd</v-icon
                                                    >
                                                </div>
                                            </v-card-title>
                                        </v-col>
                                        <v-col cols="6" align="right">
                                            <div class="mt-3">
                                                <v-icon
                                                    >mdi-dots-vertical</v-icon
                                                >
                                            </div>
                                        </v-col>
                                    </v-row>

                                    <v-card-text>
                                        <div
                                            class="text-body font-weight-bold mt-1"
                                        >
                                            Refunds
                                        </div>
                                        <div class="d-flex mt-3">
                                            <div
                                                class="text-h5 font-weight-bold"
                                            >
                                                $78
                                            </div>
                                            <div
                                                class="text-body-1 font-size-3 mx-2 pt-1"
                                                style="color: red"
                                            >
                                                -<small>15%</small>
                                            </div>
                                        </div>

                                        <div class="pt-4">Past Month</div>
                                    </v-card-text>
                                </v-card>
                            </v-col>
                        </v-row>

                        <v-row class="mt-4">
                            <v-col cols="6">
                                <v-card class="pb-1">
                                    <v-row>
                                        <v-col cols="6">
                                            <v-card-title>
                                                <div
                                                    class="bg-primary text-center pt-1"
                                                    style="
                                                        border-radius: 50%;
                                                        width: 40px;
                                                        height: 40px;
                                                        font-size: 15px;
                                                    "
                                                >
                                                    <v-icon
                                                        >mdi-package-variant-closed</v-icon
                                                    >
                                                </div>
                                            </v-card-title>
                                        </v-col>
                                        <v-col cols="6" align="right">
                                            <div class="mt-3">
                                                <v-icon
                                                    >mdi-dots-vertical</v-icon
                                                >
                                            </div>
                                        </v-col>
                                    </v-row>

                                    <v-card-text>
                                        <div
                                            class="text-body font-weight-bold mt-1"
                                        >
                                            New Project
                                        </div>
                                        <div class="d-flex mt-3">
                                            <div
                                                class="text-h5 font-weight-bold"
                                            >
                                                862
                                            </div>
                                            <div
                                                class="text-body-1 font-size-3 mx-2 pt-1"
                                                style="color: red"
                                            >
                                                -<small>18%</small>
                                            </div>
                                        </div>

                                        <div class="pt-4">Yearly Project</div>
                                    </v-card-text>
                                </v-card>
                            </v-col>

                            <v-col cols="6">
                                <v-card class="pb-1">
                                    <v-row>
                                        <v-col cols="6">
                                            <v-card-title>
                                                <div
                                                    class="bg-warning text-center pt-1"
                                                    style="
                                                        border-radius: 50%;
                                                        width: 40px;
                                                        height: 40px;
                                                        font-size: 15px;
                                                    "
                                                >
                                                    <v-icon
                                                        >mdi-help-circle-outline</v-icon
                                                    >
                                                </div>
                                            </v-card-title>
                                        </v-col>
                                        <v-col cols="6" align="right">
                                            <div class="mt-3">
                                                <v-icon
                                                    >mdi-dots-vertical</v-icon
                                                >
                                            </div>
                                        </v-col>
                                    </v-row>

                                    <v-card-text>
                                        <div
                                            class="text-body font-weight-bold mt-1"
                                        >
                                            Sale quries
                                        </div>
                                        <div class="d-flex mt-3">
                                            <div
                                                class="text-h5 font-weight-bold"
                                            >
                                                15
                                            </div>
                                            <div
                                                class="text-body-1 font-size-3 mx-2 pt-1"
                                                style="color: red"
                                            >
                                                -<small>18%</small>
                                            </div>
                                        </div>

                                        <div class="pt-4">Last Week</div>
                                    </v-card-text>
                                </v-card>
                            </v-col>
                        </v-row>
                    </v-col>
                </v-row>
            </v-col>
        </v-row>
        <v-row class="mt-8">
            <v-col cols="3">
                <v-card class="pb-5">
                    <v-row>
                        <v-col cols="7">
                            <v-card-title>Sales By Countries</v-card-title>
                        </v-col>
                        <v-col cols="5" align="right">
                            <div class="mt-3">
                                <v-icon>mdi-dots-vertical</v-icon>
                            </div>
                        </v-col>
                    </v-row>

                    <v-row>
                        <v-col cols="12">
                            <div class="d-flex justify-space-between">
                                <v-card-title class="d-flex" style="gap: 10px">
                                    <div
                                        class="bg-success text-center pt-1"
                                        style="
                                            border-radius: 50%;
                                            width: 40px;
                                            height: 40px;
                                            font-size: 15px;
                                        "
                                    >
                                        <v-icon>mdi-help-circle-outline</v-icon>
                                    </div>
                                    <div class="d-flex flex-column mt-n2">
                                        <div class="d-flex">
                                            <div
                                                class="text-body font-weight-bold"
                                            >
                                                $8,656k
                                            </div>
                                            <div
                                                class="text-body-1 font-weight-bold text-success mx-2 pt-1"
                                            >
                                                <small
                                                    ><v-icon
                                                        >mdi-chevron-up</v-icon
                                                    >25.8%</small
                                                >
                                            </div>
                                        </div>
                                        <div class="text-body-2">
                                            United States of America
                                        </div>
                                    </div>
                                </v-card-title>
                                <div class="d-flex flex-column mx-3">
                                    <div class="text-body font-weight-bold">
                                        894k
                                    </div>
                                    <div class="text-body-2 font-weight-900">
                                        Sales
                                    </div>
                                </div>
                            </div>
                        </v-col>

                        <v-col cols="12">
                            <div class="d-flex justify-space-between">
                                <v-card-title class="d-flex" style="gap: 10px">
                                    <div
                                        class="bg-success text-center pt-1"
                                        style="
                                            border-radius: 50%;
                                            width: 40px;
                                            height: 40px;
                                            font-size: 15px;
                                        "
                                    >
                                        <v-icon>mdi-help-circle-outline</v-icon>
                                    </div>
                                    <div class="d-flex flex-column mt-n2">
                                        <div class="d-flex">
                                            <div
                                                class="text-body font-weight-bold"
                                            >
                                                $8,656k
                                            </div>
                                            <div
                                                class="text-body-1 font-weight-bold text-success mx-2 pt-1"
                                            >
                                                <small
                                                    ><v-icon
                                                        >mdi-chevron-up</v-icon
                                                    >25.8%</small
                                                >
                                            </div>
                                        </div>
                                        <div class="text-body-2">
                                            United States of America
                                        </div>
                                    </div>
                                </v-card-title>
                                <div class="d-flex flex-column mx-3">
                                    <div class="text-body font-weight-bold">
                                        894k
                                    </div>
                                    <div class="text-body-2 font-weight-900">
                                        Sales
                                    </div>
                                </div>
                            </div>
                        </v-col>

                        <v-col cols="12">
                            <div class="d-flex justify-space-between">
                                <v-card-title class="d-flex" style="gap: 10px">
                                    <div
                                        class="bg-success text-center pt-1"
                                        style="
                                            border-radius: 50%;
                                            width: 40px;
                                            height: 40px;
                                            font-size: 15px;
                                        "
                                    >
                                        <v-icon>mdi-help-circle-outline</v-icon>
                                    </div>
                                    <div class="d-flex flex-column mt-n2">
                                        <div class="d-flex">
                                            <div
                                                class="text-body font-weight-bold"
                                            >
                                                $8,656k
                                            </div>
                                            <div
                                                class="text-body-1 font-weight-bold text-success mx-2 pt-1"
                                            >
                                                <small
                                                    ><v-icon
                                                        >mdi-chevron-up</v-icon
                                                    >25.8%</small
                                                >
                                            </div>
                                        </div>
                                        <div class="text-body-2">
                                            United States of America
                                        </div>
                                    </div>
                                </v-card-title>
                                <div class="d-flex flex-column mx-3">
                                    <div class="text-body font-weight-bold">
                                        894k
                                    </div>
                                    <div class="text-body-2 font-weight-900">
                                        Sales
                                    </div>
                                </div>
                            </div>
                        </v-col>
                    </v-row>
                </v-card>
            </v-col>

            <v-col cols="9">
                <v-row>
                    <v-col cols="6">
                        <v-card class="pb-5">
                            <v-row>
                                <v-col cols="7">
                                    <v-card-title>Deposit</v-card-title>
                                </v-col>
                                <v-col cols="5" align="right">
                                    <div class="mt-3 mx-3">View All</div>
                                </v-col>
                            </v-row>

                            <v-row>
                                <v-col cols="12">
                                    <div class="d-flex justify-space-between">
                                        <v-card-title
                                            class="d-flex"
                                            style="gap: 10px"
                                        >
                                            <div
                                                style="width: 50px"
                                                class="mt-n2"
                                            >
                                                <v-img
                                                    src="https://pbs.twimg.com/media/DyWXd86UwAAsLM-.png:large"
                                                ></v-img>
                                            </div>
                                            <div
                                                class="d-flex flex-column mt-n2"
                                            >
                                                <div
                                                    class="text-body font-weight-bold"
                                                >
                                                    Gumroad account
                                                </div>
                                                <div class="text-body-2">
                                                    Sell UI Kit
                                                </div>
                                            </div>
                                        </v-card-title>
                                        <div
                                            class="d-flex flex-column mx-3 pt-4"
                                        >
                                            <div
                                                class="text-body font-weight-bold mx-2 text-success"
                                            >
                                                +$4.650
                                            </div>
                                        </div>
                                    </div>
                                </v-col>

                                <v-col cols="12">
                                    <div class="d-flex justify-space-between">
                                        <v-card-title
                                            class="d-flex"
                                            style="gap: 10px"
                                        >
                                            <div
                                                style="width: 50px"
                                                class="mt-n2"
                                            >
                                                <v-img
                                                    src="https://pbs.twimg.com/media/DyWXd86UwAAsLM-.png:large"
                                                ></v-img>
                                            </div>
                                            <div
                                                class="d-flex flex-column mt-n2"
                                            >
                                                <div
                                                    class="text-body font-weight-bold"
                                                >
                                                    Gumroad account
                                                </div>
                                                <div class="text-body-2">
                                                    Sell UI Kit
                                                </div>
                                            </div>
                                        </v-card-title>
                                        <div
                                            class="d-flex flex-column mx-3 pt-4"
                                        >
                                            <div
                                                class="text-body font-weight-bold mx-2 text-success"
                                            >
                                                +$4.650
                                            </div>
                                        </div>
                                    </div>
                                </v-col>

                                <v-col cols="12">
                                    <div class="d-flex justify-space-between">
                                        <v-card-title
                                            class="d-flex"
                                            style="gap: 10px"
                                        >
                                            <div
                                                style="width: 50px"
                                                class="mt-n2"
                                            >
                                                <v-img
                                                    src="https://pbs.twimg.com/media/DyWXd86UwAAsLM-.png:large"
                                                ></v-img>
                                            </div>
                                            <div
                                                class="d-flex flex-column mt-n2"
                                            >
                                                <div
                                                    class="text-body font-weight-bold"
                                                >
                                                    Gumroad account
                                                </div>
                                                <div class="text-body-2">
                                                    Sell UI Kit
                                                </div>
                                            </div>
                                        </v-card-title>
                                        <div
                                            class="d-flex flex-column mx-3 pt-4"
                                        >
                                            <div
                                                class="text-body font-weight-bold mx-2 text-success"
                                            >
                                                +$4.650
                                            </div>
                                        </div>
                                    </div>
                                </v-col>
                            </v-row>
                        </v-card>
                    </v-col>

                    <v-col cols="6">
                        <v-card class="pb-5">
                            <v-row>
                                <v-col cols="7">
                                    <v-card-title>Withdraw</v-card-title>
                                </v-col>
                                <v-col cols="5" align="right">
                                    <div class="mt-3 mx-3">View All</div>
                                </v-col>
                            </v-row>

                            <v-row>
                                <v-col cols="12">
                                    <div class="d-flex justify-space-between">
                                        <v-card-title
                                            class="d-flex"
                                            style="gap: 10px"
                                        >
                                            <div
                                                style="width: 50px"
                                                class="mt-n2"
                                            >
                                                <v-img
                                                    src="https://pbs.twimg.com/media/DyWXd86UwAAsLM-.png:large"
                                                ></v-img>
                                            </div>
                                            <div
                                                class="d-flex flex-column mt-n2"
                                            >
                                                <div
                                                    class="text-body font-weight-bold"
                                                >
                                                    Gumroad account
                                                </div>
                                                <div class="text-body-2">
                                                    Sell UI Kit
                                                </div>
                                            </div>
                                        </v-card-title>
                                        <div
                                            class="d-flex flex-column mx-3 pt-4"
                                        >
                                            <div
                                                class="text-body font-weight-bold mx-2 text-success"
                                            >
                                                +$4.650
                                            </div>
                                        </div>
                                    </div>
                                </v-col>

                                <v-col cols="12">
                                    <div class="d-flex justify-space-between">
                                        <v-card-title
                                            class="d-flex"
                                            style="gap: 10px"
                                        >
                                            <div
                                                style="width: 50px"
                                                class="mt-n2"
                                            >
                                                <v-img
                                                    src="https://pbs.twimg.com/media/DyWXd86UwAAsLM-.png:large"
                                                ></v-img>
                                            </div>
                                            <div
                                                class="d-flex flex-column mt-n2"
                                            >
                                                <div
                                                    class="text-body font-weight-bold"
                                                >
                                                    Gumroad account
                                                </div>
                                                <div class="text-body-2">
                                                    Sell UI Kit
                                                </div>
                                            </div>
                                        </v-card-title>
                                        <div
                                            class="d-flex flex-column mx-3 pt-4"
                                        >
                                            <div
                                                class="text-body font-weight-bold mx-2 text-success"
                                            >
                                                +$4.650
                                            </div>
                                        </div>
                                    </div>
                                </v-col>

                                <v-col cols="12">
                                    <div class="d-flex justify-space-between">
                                        <v-card-title
                                            class="d-flex"
                                            style="gap: 10px"
                                        >
                                            <div
                                                style="width: 50px"
                                                class="mt-n2"
                                            >
                                                <v-img
                                                    src="https://pbs.twimg.com/media/DyWXd86UwAAsLM-.png:large"
                                                ></v-img>
                                            </div>
                                            <div
                                                class="d-flex flex-column mt-n2"
                                            >
                                                <div
                                                    class="text-body font-weight-bold"
                                                >
                                                    Gumroad account
                                                </div>
                                                <div class="text-body-2">
                                                    Sell UI Kit
                                                </div>
                                            </div>
                                        </v-card-title>
                                        <div
                                            class="d-flex flex-column mx-3 pt-4"
                                        >
                                            <div
                                                class="text-body font-weight-bold mx-2 text-success"
                                            >
                                                +$4.650
                                            </div>
                                        </div>
                                    </div>
                                </v-col>
                            </v-row>
                        </v-card>
                    </v-col>
                </v-row>
            </v-col>
        </v-row>
    </v-container>
</template>


<script>
    import { Bar } from "vue-chartjs";
    import {
        Chart as ChartJS,
        Title,
        Tooltip,
        BarElement,
        CategoryScale,
        LinearScale,
    } from "chart.js";

    ChartJS.register(Title, Tooltip, BarElement, CategoryScale, LinearScale);

    export default {
        name: "BarChart",
        components: { Bar },
        data() {
            return {
                chartData: {
                    labels: ["", "", "", "", "", "", "", ""],
                    datasets: [
                        {
                            data: [32, 60, 40, 35, 70, 60, 50, 60],
                            backgroundColor: "#7B1FA2",
                            borderColor: "#f87979",
                            borderRadius: "10px",
                        },
                    ],
                },
                chartOptions: {
                    responsive: true,
                },
            };
        },
    };
</script>