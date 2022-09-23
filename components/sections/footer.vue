<template>
    <div class="nc-Footer relative py-24 bg-gray-900 lg:py-28 border-t border-neutral-200 dark:border-neutral-700">
        <div
            class="container grid grid-cols-2 gap-y-10 gap-x-5 sm:gap-x-8 md:grid-cols-4 lg:grid-cols-5 lg:gap-x-10 ">
            <div class="grid grid-cols-4 gap-5 col-span-2 md:col-span-4 lg:md:col-span-1 lg:flex lg:flex-col">
                <div class="col-span-2 md:col-span-1"><a
                        class="ttnc-logo inline-block text-primary-6000 focus:outline-none focus:ring-0 w-24"
                        href="/chisfis/"><svg class="w-full hidden dark:block" viewBox="0 0 65 32" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M24.4444 14.0325C24.4444 21.4807 12.9444 29.3945 12.9444 29.3945C12.9444 29.3945 1.44444 21.4807 1.44444 14.0325C1.44444 7.51522 6.84722 2.39453 12.9444 2.39453C19.0417 2.39453 24.4444 7.51522 24.4444 14.0325Z"
                                fill="currentColor"></path>
                            <path
                                d="M12.9444 29.3945C12.9444 29.3945 24.4444 21.4807 24.4444 14.0325C24.4444 7.51522 19.0417 2.39453 12.9444 2.39453C6.84722 2.39453 1.44444 7.51522 1.44444 14.0325C1.44444 21.4807 12.9444 29.3945 12.9444 29.3945ZM12.9444 29.3945V2.6807"
                                stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            </path>
                            <circle cx="13" cy="15" r="4" fill="white"></circle>
                            <path
                                d="M31.8601 25.2216C32.951 25.2216 33.897 24.3097 33.9055 23.1761C33.897 22.0597 32.951 21.1477 31.8601 21.1477C30.7351 21.1477 29.8061 22.0597 29.8146 23.1761C29.8061 24.3097 30.7351 25.2216 31.8601 25.2216ZM43.9261 11.9091H41.3267V11.0312C41.3267 10.1449 41.6847 9.625 42.75 9.625C43.1847 9.625 43.6278 9.71875 43.9176 9.8125L44.5568 7.08523C44.1051 6.94886 43.108 6.72727 41.9915 6.72727C39.5284 6.72727 37.696 8.11648 37.696 10.9631V11.9091H35.8466V14.6364H37.696V25H41.3267V14.6364H43.9261V11.9091ZM46.1442 25H49.7749V11.9091H46.1442V25ZM47.968 10.2216C49.0504 10.2216 49.9368 9.39489 49.9368 8.38068C49.9368 7.375 49.0504 6.54829 47.968 6.54829C46.8942 6.54829 46.0078 7.375 46.0078 8.38068C46.0078 9.39489 46.8942 10.2216 47.968 10.2216ZM63.5753 15.642C63.2514 13.2301 61.3082 11.7386 58.0014 11.7386C54.652 11.7386 52.4446 13.2898 52.4531 15.8125C52.4446 17.7727 53.6804 19.0426 56.2372 19.554L58.5043 20.0057C59.6463 20.2358 60.1662 20.6534 60.1832 21.3097C60.1662 22.0852 59.3224 22.6392 58.0526 22.6392C56.7571 22.6392 55.8963 22.0852 55.6747 21.0199L52.1037 21.2074C52.4446 23.7131 54.5753 25.2557 58.044 25.2557C61.4361 25.2557 63.8651 23.5256 63.8736 20.9432C63.8651 19.0511 62.6293 17.9176 60.0895 17.3977L57.7202 16.9205C56.5014 16.6562 56.0497 16.2386 56.0582 15.608C56.0497 14.8239 56.9361 14.3125 58.0611 14.3125C59.3224 14.3125 60.0724 15.0028 60.2514 15.8466L63.5753 15.642Z"
                                fill="white"></path>
                        </svg><svg class="w-full block dark:hidden" viewBox="0 0 65 32" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M24.4444 14.0325C24.4444 21.4807 12.9444 29.3945 12.9444 29.3945C12.9444 29.3945 1.44444 21.4807 1.44444 14.0325C1.44444 7.51522 6.84722 2.39453 12.9444 2.39453C19.0417 2.39453 24.4444 7.51522 24.4444 14.0325Z"
                                fill="currentColor"></path>
                            <path
                                d="M12.9444 29.3945C12.9444 29.3945 24.4444 21.4807 24.4444 14.0325C24.4444 7.51522 19.0417 2.39453 12.9444 2.39453C6.84722 2.39453 1.44444 7.51522 1.44444 14.0325C1.44444 21.4807 12.9444 29.3945 12.9444 29.3945ZM12.9444 29.3945V2.6807"
                                stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            </path>
                            <circle cx="13" cy="15" r="4" fill="white"></circle>
                            <path
                                d="M31.8601 25.2216C32.951 25.2216 33.897 24.3097 33.9055 23.1761C33.897 22.0597 32.951 21.1477 31.8601 21.1477C30.7351 21.1477 29.8061 22.0597 29.8146 23.1761C29.8061 24.3097 30.7351 25.2216 31.8601 25.2216ZM43.9261 11.9091H41.3267V11.0312C41.3267 10.1449 41.6847 9.625 42.75 9.625C43.1847 9.625 43.6278 9.71875 43.9176 9.8125L44.5568 7.08523C44.1051 6.94886 43.108 6.72727 41.9915 6.72727C39.5284 6.72727 37.696 8.11648 37.696 10.9631V11.9091H35.8466V14.6364H37.696V25H41.3267V14.6364H43.9261V11.9091ZM46.1442 25H49.7749V11.9091H46.1442V25ZM47.968 10.2216C49.0504 10.2216 49.9368 9.39489 49.9368 8.38068C49.9368 7.375 49.0504 6.54829 47.968 6.54829C46.8942 6.54829 46.0078 7.375 46.0078 8.38068C46.0078 9.39489 46.8942 10.2216 47.968 10.2216ZM63.5753 15.642C63.2514 13.2301 61.3082 11.7386 58.0014 11.7386C54.652 11.7386 52.4446 13.2898 52.4531 15.8125C52.4446 17.7727 53.6804 19.0426 56.2372 19.554L58.5043 20.0057C59.6463 20.2358 60.1662 20.6534 60.1832 21.3097C60.1662 22.0852 59.3224 22.6392 58.0526 22.6392C56.7571 22.6392 55.8963 22.0852 55.6747 21.0199L52.1037 21.2074C52.4446 23.7131 54.5753 25.2557 58.044 25.2557C61.4361 25.2557 63.8651 23.5256 63.8736 20.9432C63.8651 19.0511 62.6293 17.9176 60.0895 17.3977L57.7202 16.9205C56.5014 16.6562 56.0497 16.2386 56.0582 15.608C56.0497 14.8239 56.9361 14.3125 58.0611 14.3125C59.3224 14.3125 60.0724 15.0028 60.2514 15.8466L63.5753 15.642Z"
                                fill="#1F2937"></path>
                        </svg></a></div>
                <div class="col-span-2 flex items-center md:col-span-3">
                    <div class="nc-SocialsList1 flex items-center space-x-3 lg:space-x-0 lg:flex-col lg:space-y-2.5 lg:items-start"
                        data-nc-id="SocialsList1"><a href="#"
                            class="flex items-center text-2xl text-neutral-700 hover:text-black dark:text-neutral-300 dark:hover:text-white leading-none space-x-2 group"><i
                                class="lab la-facebook-square"></i><span
                                class="hidden lg:block text-sm">Facebook</span></a><a href="#"
                            class="flex items-center text-2xl text-neutral-700 hover:text-black dark:text-neutral-300 dark:hover:text-white leading-none space-x-2 group"><i
                                class="lab la-twitter"></i><span
                                class="hidden lg:block text-sm">Twitter</span></a><a href="#"
                            class="flex items-center text-2xl text-neutral-700 hover:text-black dark:text-neutral-300 dark:hover:text-white leading-none space-x-2 group"><i
                                class="lab la-youtube"></i><span
                                class="hidden lg:block text-sm">Youtube</span></a><a href="#"
                            class="flex items-center text-2xl text-neutral-700 hover:text-black dark:text-neutral-300 dark:hover:text-white leading-none space-x-2 group"><i
                                class="lab la-instagram"></i><span
                                class="hidden lg:block text-sm">Instagram</span></a></div>
                </div>
            </div>
            <div class="text-sm">
                <h2 class="font-semibold text-neutral-700 dark:text-neutral-200">Getting started</h2>
                <ul class="mt-5 space-y-4">
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Installation</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Release Notes</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Upgrade Guide</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Browser Support</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Editor Support</a></li>
                </ul>
            </div>
            <div class="text-sm">
                <h2 class="font-semibold text-neutral-700 dark:text-neutral-200">Explore</h2>
                <ul class="mt-5 space-y-4">
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Design features</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Prototyping</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Design systems</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Pricing</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Security</a></li>
                </ul>
            </div>
            <div class="text-sm">
                <h2 class="font-semibold text-neutral-700 dark:text-neutral-200">Resources</h2>
                <ul class="mt-5 space-y-4">
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Best practices</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Support</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Developers</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Learn design</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Releases</a></li>
                </ul>
            </div>
            <div class="text-sm">
                <h2 class="font-semibold text-neutral-700 dark:text-neutral-200">Community</h2>
                <ul class="mt-5 space-y-4">
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Discussion Forums</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Code of Conduct</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Community Resources</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Contributing</a></li>
                    <li><a class="text-neutral-6000 dark:text-neutral-300 hover:text-black dark:hover:text-white"
                            href="#">Concurrent Mode</a></li>
                </ul>
            </div>
        </div>
    </div>
</template>