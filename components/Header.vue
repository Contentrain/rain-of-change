<template>
  <header class="app-header fixed w-full h-24 top-0 border-b-2 border-gray-100 bg-white z-10">
    <nav class="max-w-2xl px-4 py-6 m-auto flex justify-between">
      <a
        class="logo-container flex items-center"
        href="https://contentrain.io"
        target="_blank"
        rel="noopener noreferrer"
      >
        <div class="logo-icon">
          <svg
            width="48"
            height="48"
            viewBox="0 0 48 48"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink"
          >
            <rect width="48" height="48" rx="6" fill="url(#pattern0)" />
            <defs>
              <pattern
                id="pattern0"
                patternContentUnits="objectBoundingBox"
                width="1"
                height="1"
              >
                <use
                  xlink:href="#image0_32_10309"
                  transform="scale(0.015625)"
                />
              </pattern>
              <image
                id="image0_32_10309"
                width="64"
                height="64"
                xlink:href="data:image/png;base64,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"
              />
            </defs>
          </svg>
        </div>
        <div class="logo-text text-gray-400 ml-4">
          <div>
            <svg
              width="93"
              height="13"
              viewBox="0 0 93 13"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M10.416 9.088L8.384 8.48C8.048 9.744 7.216 10.352 5.952 10.352C4.176 10.352 3.136 9.056 3.136 6.72C3.136 4.368 4.24 3.088 6 3.088C7.216 3.088 7.92 3.584 8.272 4.864L10.272 4.016C9.68 2.176 8.064 1.28 5.904 1.28C2.816 1.28 0.848 3.328 0.848 6.72C0.848 10.112 2.8 12.16 5.936 12.16C8.08 12.16 9.776 11.152 10.416 9.088ZM15.7539 3.84C13.1779 3.84 11.6579 5.392 11.6579 8C11.6579 10.608 13.1779 12.16 15.7539 12.16C18.3299 12.16 19.8499 10.608 19.8499 8C19.8499 5.392 18.3299 3.84 15.7539 3.84ZM15.7539 5.472C16.9859 5.472 17.6579 6.304 17.6579 8C17.6579 9.696 16.9859 10.528 15.7539 10.528C14.5219 10.528 13.8499 9.696 13.8499 8C13.8499 6.304 14.5219 5.472 15.7539 5.472ZM26.4981 3.84C25.2981 3.84 24.3061 4.352 23.7781 5.424L23.6981 4H21.7301V12H23.9221V7.776C23.9221 6.176 24.8341 5.568 25.7621 5.568C26.5941 5.568 27.1861 6.016 27.1861 7.392V12H29.3781V6.752C29.3781 4.816 28.1621 3.84 26.4981 3.84ZM36.7259 10.048C36.3899 10.336 36.0219 10.496 35.4939 10.496C34.8059 10.496 34.3899 10.16 34.3899 9.392V5.632H36.9819V4H34.3899V1.552L32.1979 2.16V4H30.7419V5.632H32.1979V9.744C32.1979 11.504 33.2859 12.16 34.8699 12.16C35.7179 12.16 36.5499 11.92 37.0619 11.504L36.7259 10.048ZM45.9053 7.968C45.9053 5.344 44.5453 3.84 42.0493 3.84C39.4733 3.84 38.0173 5.376 38.0173 8C38.0173 10.624 39.5213 12.16 42.1773 12.16C43.9853 12.16 45.2173 11.472 45.7292 10.192L43.9373 9.536C43.7133 10.176 43.1053 10.528 42.1773 10.528C41.1053 10.528 40.4013 9.984 40.1773 8.832H45.8413C45.8733 8.624 45.9053 8.192 45.9053 7.968ZM42.0333 5.456C43.0413 5.456 43.7133 6.096 43.8893 7.296H40.1613C40.3373 6.08 40.9773 5.456 42.0333 5.456ZM52.5138 3.84C51.3138 3.84 50.3218 4.352 49.7938 5.424L49.7138 4H47.7458V12H49.9378V7.776C49.9378 6.176 50.8498 5.568 51.7778 5.568C52.6098 5.568 53.2018 6.016 53.2018 7.392V12H55.3938V6.752C55.3938 4.816 54.1778 3.84 52.5138 3.84ZM62.7415 10.048C62.4055 10.336 62.0375 10.496 61.5095 10.496C60.8215 10.496 60.4055 10.16 60.4055 9.392V5.632H62.9975V4H60.4055V1.552L58.2135 2.16V4H56.7575V5.632H58.2135V9.744C58.2135 11.504 59.3015 12.16 60.8855 12.16C61.7335 12.16 62.5655 11.92 63.0775 11.504L62.7415 10.048ZM68.9769 3.84C67.7289 3.84 66.9129 4.464 66.4969 5.568L66.3529 4H64.4489V12H66.6409V7.856C66.6409 6.4 67.6009 5.696 68.5609 5.696C68.9769 5.696 69.3449 5.792 69.5689 5.936L69.8409 4.016C69.6489 3.904 69.3289 3.84 68.9769 3.84ZM78.3703 10.672C77.9543 10.672 77.7783 10.48 77.7783 10.064V6.784C77.7783 4.8 76.3703 3.84 74.1463 3.84C72.1943 3.84 70.9943 4.704 70.6583 6.064L72.4023 6.8C72.6423 5.792 73.3143 5.44 74.2423 5.44C75.1063 5.44 75.6023 5.984 75.6023 6.832V7.216L73.6823 7.584C71.5383 7.984 70.5623 8.864 70.5623 10.112C70.5623 11.456 71.5223 12.16 73.0423 12.16C74.3863 12.16 75.3943 11.744 75.8743 10.96C76.0983 11.824 76.7543 12.16 77.7143 12.16C78.1143 12.16 78.4663 12.08 78.7543 11.936L78.9143 10.608C78.7543 10.656 78.5623 10.672 78.3703 10.672ZM73.7303 10.672C73.1543 10.672 72.8183 10.4 72.8183 9.888C72.8183 9.36 73.1863 9.104 73.8903 8.944L75.6023 8.56V9.392C75.6023 10.24 74.5623 10.672 73.7303 10.672ZM81.3498 2.848C82.2618 2.848 82.7098 2.464 82.7098 1.68C82.7098 0.896 82.2618 0.495999 81.3498 0.495999C80.4378 0.495999 79.9898 0.896 79.9898 1.68C79.9898 2.464 80.4378 2.848 81.3498 2.848ZM82.4378 4H80.2458V12H82.4378V4ZM89.5294 3.84C88.3294 3.84 87.3374 4.352 86.8094 5.424L86.7294 4H84.7614V12H86.9534V7.776C86.9534 6.176 87.8654 5.568 88.7934 5.568C89.6254 5.568 90.2174 6.016 90.2174 7.392V12H92.4094V6.752C92.4094 4.816 91.1934 3.84 89.5294 3.84Z"
                fill="#37393C"
              />
            </svg>
          </div>
          <div>
            <small>contentrain.io</small>
          </div>
        </div>
      </a>
      <div class="social-icons text-gray-400 flex items-center text-xl">
        <a class="ml-4 hover:text-blue-500" href="https://github.com/Contentrain/rain-of-change.git" target="_blank" rel="noopener noreferrer">
          <i class="ri-github-fill" />
        </a>
        <a class="ml-4 hover:text-blue-500" href="https://twitter.com/contentrain_io" target="_blank" rel="noopener noreferrer">
          <i class="ri-twitter-fill" />
        </a>
        <a class="ml-4 hover:text-blue-500" href="https://www.linkedin.com/company/contentrain" target="_blank" rel="noopener noreferrer">
          <i class="ri-linkedin-fill" />
        </a>
      </div>
    </nav>
  </header>
</template>
