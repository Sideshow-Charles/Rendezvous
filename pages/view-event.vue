<template>
    <div>
        <div class="view__event">
            <!-- Header Component -->
            <div class="header__container">
                <Header headerStyle="view-event__header"></Header>
            </div>
            <!-- End of Header Container -->

            <div class="hero__image__container">
                <img src="../assets/images/view-event-image.png" alt="Hero Image For Event">
            </div>

            <!-- Event Description -->
            <section class="event__details__container">
                <section class="event__details__left">
                    <p class="event__name">I said what I said Live Show</p>
                    <div class="event__date_and__time__container">
                        <div class="event__date"><svg width="24" height="24" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <rect width="24" height="24" fill="white" style="mix-blend-mode:multiply" />
                                <path
                                    d="M19.5 3H16.5V1.5H15V3H9V1.5H7.5V3H4.5C3.675 3 3 3.675 3 4.5V19.5C3 20.325 3.675 21 4.5 21H19.5C20.325 21 21 20.325 21 19.5V4.5C21 3.675 20.325 3 19.5 3ZM19.5 19.5H4.5V9H19.5V19.5ZM19.5 7.5H4.5V4.5H7.5V6H9V4.5H15V6H16.5V4.5H19.5V7.5Z"
                                    fill="#9B51E0" />
                            </svg>
                            <p>Sunday, October 3rd, 2023</p>
                        </div>
                        <div class="event__time"><svg width="24" height="24" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <rect width="24" height="24" fill="white" style="mix-blend-mode:multiply" />
                                <path
                                    d="M12 22.5C9.9233 22.5 7.89323 21.8842 6.16652 20.7304C4.4398 19.5767 3.09399 17.9368 2.29927 16.0182C1.50455 14.0996 1.29661 11.9884 1.70176 9.95156C2.1069 7.91476 3.10693 6.04383 4.57538 4.57538C6.04383 3.10693 7.91476 2.1069 9.95156 1.70176C11.9884 1.29661 14.0996 1.50455 16.0182 2.29927C17.9368 3.09399 19.5767 4.4398 20.7304 6.16652C21.8842 7.89323 22.5 9.9233 22.5 12C22.5 14.7848 21.3938 17.4555 19.4246 19.4246C17.4555 21.3938 14.7848 22.5 12 22.5ZM12 3C10.22 3 8.47992 3.52785 6.99987 4.51678C5.51983 5.50571 4.36628 6.91132 3.68509 8.55585C3.0039 10.2004 2.82567 12.01 3.17294 13.7558C3.5202 15.5016 4.37737 17.1053 5.63604 18.364C6.89472 19.6226 8.49836 20.4798 10.2442 20.8271C11.99 21.1743 13.7996 20.9961 15.4442 20.3149C17.0887 19.6337 18.4943 18.4802 19.4832 17.0001C20.4722 15.5201 21 13.78 21 12C21 9.61306 20.0518 7.32387 18.364 5.63604C16.6761 3.94822 14.387 3 12 3Z"
                                    fill="#9B51E0" />
                                <path d="M15.4425 16.5L11.25 12.3075V5.25H12.75V11.685L16.5 15.4425L15.4425 16.5Z"
                                    fill="#9B51E0" />
                            </svg>
                            <p>6PM</p>
                        </div>
                    </div>
                    <div class="event__address"><svg width="24" height="24" viewBox="0 0 24 24" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <rect width="24" height="24" fill="white" style="mix-blend-mode:multiply" />
                            <path
                                d="M12 13.5C11.2583 13.5 10.5333 13.2801 9.91662 12.868C9.29994 12.456 8.81929 11.8703 8.53546 11.1851C8.25163 10.4998 8.17737 9.74584 8.32206 9.01841C8.46676 8.29098 8.82391 7.6228 9.34836 7.09835C9.8728 6.5739 10.541 6.21675 11.2684 6.07205C11.9958 5.92736 12.7498 6.00162 13.4351 6.28545C14.1203 6.56928 14.706 7.04993 15.118 7.66661C15.5301 8.2833 15.75 9.00832 15.75 9.75C15.7489 10.7442 15.3534 11.6974 14.6504 12.4004C13.9474 13.1034 12.9942 13.4989 12 13.5ZM12 7.5C11.555 7.5 11.12 7.63196 10.75 7.87919C10.38 8.12643 10.0916 8.47783 9.92128 8.88896C9.75098 9.3001 9.70642 9.7525 9.79324 10.189C9.88006 10.6254 10.0943 11.0263 10.409 11.341C10.7237 11.6557 11.1246 11.87 11.5611 11.9568C11.9975 12.0436 12.4499 11.999 12.861 11.8287C13.2722 11.6584 13.6236 11.37 13.8708 11C14.118 10.63 14.25 10.195 14.25 9.75C14.2494 9.15346 14.0121 8.58155 13.5903 8.15973C13.1685 7.73792 12.5965 7.50066 12 7.5Z"
                                fill="#9B51E0" />
                            <path
                                d="M12 22.5L5.67338 15.0385C5.63746 14.9956 5.41223 14.6999 5.41223 14.6999C4.33141 13.2763 3.74748 11.5374 3.75001 9.75C3.75001 7.56196 4.6192 5.46354 6.16638 3.91637C7.71355 2.36919 9.81197 1.5 12 1.5C14.188 1.5 16.2865 2.36919 17.8336 3.91637C19.3808 5.46354 20.25 7.56196 20.25 9.75C20.2527 11.5367 19.6692 13.2749 18.5889 14.698L18.5878 14.6999C18.5878 14.6999 18.3628 14.9956 18.3293 15.0354L12 22.5ZM6.60938 13.7963C6.60938 13.7963 6.78443 14.0274 6.82433 14.077L12 20.1809L17.1825 14.0684C17.2154 14.027 17.3916 13.7942 17.3916 13.7942C18.2746 12.631 18.7517 11.2103 18.75 9.75C18.75 7.95979 18.0388 6.2429 16.773 4.97703C15.5071 3.71116 13.7902 3 12 3C10.2098 3 8.49291 3.71116 7.22704 4.97703C5.96117 6.2429 5.25001 7.95979 5.25001 9.75C5.24835 11.2111 5.72587 12.6325 6.60938 13.7963Z"
                                fill="#9B51E0" />
                        </svg>
                        <p>Race Course, 8/9 Marina, Onikan, Lagos Lagos, 4aa Force Rd, Lagos Island 102273, Lagos</p>
                    </div>

                    <div class="event__organizer">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect width="24" height="24" fill="white" style="mix-blend-mode:multiply" />
                            <path
                                d="M12 3C12.7417 3 13.4667 3.21993 14.0834 3.63199C14.7001 4.04404 15.1807 4.62971 15.4645 5.31494C15.7484 6.00016 15.8226 6.75416 15.6779 7.48159C15.5333 8.20902 15.1761 8.8772 14.6517 9.40165C14.1272 9.9261 13.459 10.2833 12.7316 10.4279C12.0042 10.5726 11.2502 10.4984 10.5649 10.2145C9.87971 9.93072 9.29404 9.45007 8.88199 8.83339C8.46993 8.2167 8.25 7.49168 8.25 6.75C8.25 5.75544 8.64509 4.80161 9.34835 4.09835C10.0516 3.39509 11.0054 3 12 3ZM12 1.5C10.9616 1.5 9.94661 1.80791 9.08326 2.38478C8.2199 2.96166 7.54699 3.7816 7.14963 4.74091C6.75227 5.70022 6.64831 6.75582 6.85088 7.77422C7.05345 8.79262 7.55346 9.72808 8.28769 10.4623C9.02192 11.1965 9.95738 11.6966 10.9758 11.8991C11.9942 12.1017 13.0498 11.9977 14.0091 11.6004C14.9684 11.203 15.7883 10.5301 16.3652 9.66674C16.9421 8.80339 17.25 7.78835 17.25 6.75C17.25 5.35761 16.6969 4.02226 15.7123 3.03769C14.7277 2.05312 13.3924 1.5 12 1.5Z"
                                fill="#9B51E0" />
                            <path
                                d="M19.5 22.5H18V18.75C18 18.2575 17.903 17.7699 17.7145 17.3149C17.5261 16.86 17.2499 16.4466 16.9017 16.0983C16.5534 15.7501 16.14 15.4739 15.6851 15.2855C15.2301 15.097 14.7425 15 14.25 15H9.75C8.75544 15 7.80161 15.3951 7.09835 16.0983C6.39509 16.8016 6 17.7554 6 18.75V22.5H4.5V18.75C4.5 17.3576 5.05312 16.0223 6.03769 15.0377C7.02226 14.0531 8.35761 13.5 9.75 13.5H14.25C15.6424 13.5 16.9777 14.0531 17.9623 15.0377C18.9469 16.0223 19.5 17.3576 19.5 18.75V22.5Z"
                                fill="#9B51E0" />
                        </svg>
                        <p>FK, Jollz</p>
                    </div>

                    <article class="event__description__container">
                        <article class="event__description__header">Event description</article>
                        <article class="event__description__text">Lorem ipsum dolor sit amet, consectetur adipiscing elit,
                            sed
                            do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
                            nostrud
                            exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
                            reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
                            occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
                            labore
                            et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi
                            ut
                            aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
                            cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
                            culpa qui officia deserunt mollit anim id est laborum.Lorem ipsum dolor sit amet, consectetur
                            adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
                            minim
                            veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis
                            aute
                            irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                            Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim
                            id
                            est laborum.
                        </article>
                    </article>
                    <section class="ticket__container">
                        <p class="ticket__header">Tickets Pricing</p>

                        <!-- Ticket Container -->
                        <section class="ticket__card__container">
                            <!-- Single Ticket Price Container -->
                            <div class="single__ticket__container">
                                <p class="single__ticket__header">Single</p>
                                <p class="single__ticket__price">NGN 5,000</p>
                            </div>
                            <!-- End of Single Ticket Price Container -->

                            <!-- Pair Ticket Price Container -->
                            <div class="pair__ticket__container">
                                <p class="pair__ticket__header">Pair</p>
                                <p class="pair__ticket__price">NGN 9,000</p>
                            </div>
                            <!-- End of Pair Ticket Price Container -->
                        </section>
                        <!-- Ticket Container -->
                    </section>
                </section>
                <section class="event__details__right">
                    <section class="social__links__container">
                        <section class="social__links__header">Contact Organizers</section>
                        <section class="social__links__icons__container">
                            <section class="social__links__icons">
                                <svg width="32" height="32" viewBox="0 0 32 32" fill="none"
                                    xmlns="http://www.w3.org/2000/svg">
                                    <path
                                        d="M16 0C18.2095 0 20.2857 0.419048 22.2286 1.25714C24.1714 2.09524 25.8667 3.2381 27.3143 4.68571C28.7619 6.13333 29.9048 7.82857 30.7429 9.77143C31.581 11.7143 32 13.7905 32 16C32 18.2095 31.581 20.2857 30.7429 22.2286C29.9048 24.1714 28.7619 25.8667 27.3143 27.3143C25.8667 28.7619 24.1714 29.9048 22.2286 30.7429C20.2857 31.581 18.2095 32 16 32C13.7905 32 11.7143 31.581 9.77143 30.7429C7.82857 29.9048 6.13333 28.7619 4.68571 27.3143C3.2381 25.8667 2.09524 24.1714 1.25714 22.2286C0.419048 20.2857 0 18.2095 0 16C0 13.7905 0.419048 11.7143 1.25714 9.77143C2.09524 7.82857 3.2381 6.13333 4.68571 4.68571C6.13333 3.2381 7.82857 2.09524 9.77143 1.25714C11.7143 0.419048 13.7905 0 16 0ZM7.00952 20.1524L11.8095 16.7238L7.00952 13.2952V20.1524ZM24.9905 21.6762L19.1238 17.4857L16 19.7333L12.8381 17.4857L7.00952 21.6762V24H24.9905V21.6762ZM24.9905 13.2952L20.1905 16.7238L24.9905 20.1524V13.2952ZM24.9905 8H7.00952V10.3238L16 16.7238L24.9905 10.3238V8Z"
                                        fill="#783EAD" />
                                </svg>
                                <svg width="32" height="32" viewBox="0 0 32 32" fill="none"
                                    xmlns="http://www.w3.org/2000/svg">
                                    <path
                                        d="M24.0096 0C25.1055 0 26.1378 0.210275 27.1063 0.630824C28.0749 1.05137 28.9223 1.62485 29.6487 2.35125C30.3751 3.07766 30.9486 3.92513 31.3692 4.89367C31.7897 5.86221 32 6.89446 32 7.99044V23.9713C32 25.0673 31.7897 26.1059 31.3692 27.0872C30.9486 28.0685 30.3751 28.9223 29.6487 29.6487C28.9223 30.3751 28.0749 30.9486 27.1063 31.3692C26.1378 31.7897 25.1055 32 24.0096 32H7.99044C6.89446 32 5.86221 31.7897 4.89367 31.3692C3.92513 30.9486 3.07766 30.3751 2.35125 29.6487C1.62485 28.9223 1.05137 28.0685 0.630824 27.0872C0.210275 26.1059 0 25.0673 0 23.9713V7.99044C0 6.89446 0.210275 5.86221 0.630824 4.89367C1.05137 3.92513 1.62485 3.07766 2.35125 2.35125C3.07766 1.62485 3.92513 1.05137 4.89367 0.630824C5.86221 0.210275 6.89446 0 7.99044 0H24.0096ZM23.6272 12.043C24.3664 11.5333 25.0163 10.8706 25.5771 10.055C25.2202 10.2079 24.857 10.3353 24.4875 10.4373C24.1179 10.5392 23.7419 10.6157 23.3596 10.6667C24.2007 10.1314 24.7614 9.40502 25.0418 8.48746C24.2772 8.97172 23.4616 9.29032 22.595 9.44325C21.8303 8.62764 20.8746 8.21983 19.7276 8.21983C19.1924 8.21983 18.689 8.32178 18.2174 8.52569C17.7459 8.72959 17.3381 9.00996 16.994 9.36679C16.6499 9.72362 16.3759 10.1378 16.172 10.6093C15.9681 11.0808 15.8662 11.5842 15.8662 12.1195C15.8662 12.2724 15.8726 12.419 15.8853 12.5591C15.898 12.6993 15.9172 12.8459 15.9427 12.9988C14.3369 12.9223 12.8459 12.5209 11.4695 11.7945C10.0932 11.0681 8.92075 10.1187 7.95221 8.94624C7.59538 9.53246 7.41697 10.1824 7.41697 10.8961C7.41697 11.5587 7.57626 12.1704 7.89486 12.7312C8.21346 13.2919 8.62764 13.7507 9.13739 14.1075C8.83154 14.1075 8.53206 14.0629 8.23895 13.9737C7.94584 13.8845 7.6591 13.7762 7.37873 13.6487V13.687C7.37873 14.63 7.67822 15.452 8.27718 16.1529C8.87614 16.8538 9.62166 17.3063 10.5137 17.5102C10.1569 17.5866 9.81282 17.6248 9.48148 17.6248H9.11828L8.75508 17.5484C9.00996 18.3385 9.46237 18.9821 10.1123 19.4791C10.7622 19.9761 11.5205 20.2374 12.3871 20.2628C11.7244 20.7726 10.9789 21.1804 10.1505 21.4863C9.32218 21.7921 8.46197 21.945 7.56989 21.945C7.39148 21.945 7.22581 21.9387 7.07288 21.9259C6.91995 21.9132 6.76702 21.8941 6.6141 21.8686C7.48068 22.4293 8.41736 22.8626 9.42413 23.1685C10.4309 23.4743 11.4823 23.6272 12.5783 23.6272C14.3624 23.6272 15.9427 23.2895 17.319 22.6141C18.6953 21.9387 19.8487 21.0721 20.779 20.0143C21.7093 18.9566 22.4166 17.7714 22.9008 16.4588C23.3851 15.1462 23.6272 13.8399 23.6272 12.54V12.043Z"
                                        fill="#783EAD" />
                                </svg>
                                <svg width="32" height="32" viewBox="0 0 32 32" fill="none"
                                    xmlns="http://www.w3.org/2000/svg">
                                    <path
                                        d="M21.4098 16.0191C21.4098 15.5858 21.3461 15.1143 21.2186 14.6045H22.8244V22.3274C22.8244 22.5313 22.7543 22.6969 22.6141 22.8244C22.4739 22.9518 22.3019 23.0155 22.098 23.0155H9.51971C9.31581 23.0155 9.15014 22.9518 9.0227 22.8244C8.89526 22.6969 8.83154 22.5313 8.83154 22.3274V14.6045H10.399C10.2716 15.1143 10.2079 15.5858 10.2079 16.0191C10.2079 16.7838 10.3544 17.5102 10.6476 18.1983C10.9407 18.8865 11.3421 19.4791 11.8519 19.9761C12.3616 20.4731 12.9606 20.8682 13.6487 21.1613C14.3369 21.4544 15.0633 21.601 15.828 21.601C16.5926 21.601 17.319 21.4544 18.0072 21.1613C18.6953 20.8682 19.2879 20.4731 19.7849 19.9761C20.282 19.4791 20.677 18.8865 20.9701 18.1983C21.2632 17.5102 21.4098 16.7838 21.4098 16.0191ZM15.828 19.4982C15.3437 19.4982 14.8849 19.409 14.4516 19.2306C14.0183 19.0522 13.6424 18.8037 13.3238 18.4851C13.0052 18.1665 12.7567 17.7969 12.5783 17.3763C12.3998 16.9558 12.3106 16.5034 12.3106 16.0191C12.3106 15.5348 12.3998 15.0761 12.5783 14.6428C12.7567 14.2095 13.0052 13.8335 13.3238 13.5149C13.6424 13.1963 14.0183 12.9478 14.4516 12.7694C14.8849 12.591 15.3437 12.5018 15.828 12.5018C16.3122 12.5018 16.7646 12.591 17.1852 12.7694C17.6057 12.9478 17.9753 13.1963 18.2939 13.5149C18.6125 13.8335 18.861 14.2095 19.0394 14.6428C19.2178 15.0761 19.307 15.5348 19.307 16.0191C19.307 16.5034 19.2178 16.9558 19.0394 17.3763C18.861 17.7969 18.6125 18.1665 18.2939 18.4851C17.9753 18.8037 17.6057 19.0522 17.1852 19.2306C16.7646 19.409 16.3122 19.4982 15.828 19.4982ZM22.098 9.0227C22.3019 9.0227 22.4739 9.08642 22.6141 9.21386C22.7543 9.3413 22.8244 9.50697 22.8244 9.71087V11.8136C22.8244 12.0175 22.7543 12.1832 22.6141 12.3106C22.4739 12.4381 22.3019 12.5018 22.098 12.5018H19.9952C19.7913 12.5018 19.6256 12.4381 19.4982 12.3106C19.3708 12.1832 19.307 12.0175 19.307 11.8136V9.71087C19.307 9.50697 19.3708 9.3413 19.4982 9.21386C19.6256 9.08642 19.7913 9.0227 19.9952 9.0227H22.098ZM23.9713 0C25.0673 0 26.1059 0.210275 27.0872 0.630824C28.0685 1.05137 28.9223 1.62485 29.6487 2.35125C30.3751 3.07766 30.9486 3.92513 31.3692 4.89367C31.7897 5.86221 32 6.89446 32 7.99044V23.9713C32 25.0673 31.7897 26.1059 31.3692 27.0872C30.9486 28.0685 30.3751 28.9223 29.6487 29.6487C28.9223 30.3751 28.0685 30.9486 27.0872 31.3692C26.1059 31.7897 25.0673 32 23.9713 32H7.99044C6.89446 32 5.86221 31.7897 4.89367 31.3692C3.92513 30.9486 3.07766 30.3751 2.35125 29.6487C1.62485 28.9223 1.05137 28.0685 0.630824 27.0872C0.210275 26.1059 0 25.0673 0 23.9713V7.99044C0 6.89446 0.210275 5.86221 0.630824 4.89367C1.05137 3.92513 1.62485 3.07766 2.35125 2.35125C3.07766 1.62485 3.92513 1.05137 4.89367 0.630824C5.86221 0.210275 6.89446 0 7.99044 0H23.9713ZM24.9271 9.0227C24.9271 8.43648 24.7232 7.93947 24.3154 7.53166C23.9076 7.12385 23.4106 6.91995 22.8244 6.91995H8.83154C8.24532 6.91995 7.74831 7.12385 7.3405 7.53166C6.9327 7.93947 6.72879 8.43648 6.72879 9.0227V23.0155C6.72879 23.6018 6.9327 24.0988 7.3405 24.5066C7.74831 24.9144 8.24532 25.1183 8.83154 25.1183H22.8244C23.4106 25.1183 23.9076 24.9144 24.3154 24.5066C24.7232 24.0988 24.9271 23.6018 24.9271 23.0155V9.0227Z"
                                        fill="#783EAD" />
                                </svg>
                            </section>
                        </section>
                    </section>
                </section>
            </section>
            <!-- Event Description -->
        </div>
        <!-- Footer Component -->
        <Footer></Footer>
        <!-- End Of Footer Component-->
    </div>
</template>

<script>
import Header from "../components/Header";
import Footer from "../components/Footer"
export default {
    components: Header,
    Footer

}
</script>

<style scoped>
.view__event {
    max-width: 90rem;
    margin: 0 auto;
    padding: 0;
}

.hero__image__container {
    padding: 0 64px;
}

.hero__image__container img {
    width: 100%;
    height: 100%;
    border-radius: 10px;
}

.event__details__container {
    margin-top: 48px;
    padding: 0 64px;
    /* display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 37px; */
}

/* .event__details__left {
    width: 75%;
} */

.event__name {
    color: #000;
    font-family: 'Gilroy-Medium ☞';
    font-size: 24px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    padding-bottom: 16px;
}

.event__date_and__time__container {
    display: flex;
    gap: 24px;
    align-items: center;
    padding-bottom: 13px;
}

.event__date {
    display: flex;
    align-items: center;
    gap: 6px;
    color: #000;
    font-family: 'Gilroy-Regular ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.event__time {
    display: flex;
    align-items: center;
    gap: 6px;
    color: #000;
    font-family: 'Gilroy-Regular ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.event__address {
    display: flex;
    align-items: center;
    gap: 6px;
    color: #000;
    font-family: 'Gilroy-Regular ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    padding-bottom: 13px;
}

.event__organizer {
    display: flex;
    align-items: center;
    gap: 6px;
    color: #000;
    font-family: 'Gilroy-Regular ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.event__description__container {
    padding-top: 53px;
    padding-bottom: 40px;
}

.event__description__header {
    color: #000;
    font-family: 'Gilroy-Medium ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    padding-bottom: 20px;
}

.event__description__text {
    color: #000;
    font-family: 'Gilroy-Light ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: 1.5;
    /* width: 75%; */
}

.ticket__container {
    padding-top: 20px;
}

.ticket__header {
    color: #000;
    font-family: 'Gilroy-Medium ☞';
    font-size: 20px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.ticket__card__container {
    padding: 20px 0;
    display: flex;
    align-items: center;
    gap: 52px;
}

.single__ticket__header {
    color: #000;
    font-family: 'Gilroy-Medium ☞';
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    padding-bottom: 8px
}

.single__ticket__price {
    color: #9B51E0;
    font-family: 'Gilroy-Medium ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.pair__ticket__header {
    color: #000;
    font-family: 'Gilroy-Medium ☞';
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    padding-bottom: 8px
}

.pair__ticket__price {
    color: #9B51E0;
    font-family: 'Gilroy-Medium ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.social__links__header {
    color: #000;
    font-family: 'Gilroy-Medium ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    padding-bottom: 20px;
}

.social__links__icons {
    display: flex;
    gap: 24px;
}

.social__links__container {
    padding-top: 50px;
    padding-bottom: 141px;
}

/* Media Queries */
@media screen and (max-width: 968px) {
    .hero__image__container {
        padding-top: 50px;
    }
}

@media screen and (max-width: 768px) {

    .hero__image__container,
    .event__details__container {
        padding-left: 16px;
        padding-right: 16px;
    }
    .hero__image__container img {
    width: 100%;
    }
}

/* @media screen and (max-width: 540px) {

    .hero__image__container,
    .event__details__container {
        padding-left: 16px;
        padding-right: 16px;
    }

    .hero__image__container img {
    width: 100%;
    border-radius: 10px;
} */

</style>
