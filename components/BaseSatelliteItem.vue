<template>  
            <div class="satellite-info">
              <div class="satellite-icon">
                <svg width="50" height="50" viewBox="0 0 50 50" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M39.5833 40.0833H40.0833V39.5833V10.4167V9.91667H39.5833H10.4167H9.91667V10.4167V39.5833V40.0833H10.4167H39.5833ZM13.5235 34.9167L18.7622 28.1937L22.8235 33.09L23.2215 33.5699L23.6035 33.0772L29.452 25.5326L36.4992 34.9167H13.5235ZM10.4167 6.75H39.5833C41.5989 6.75 43.25 8.40114 43.25 10.4167V39.5833C43.25 41.5989 41.5989 43.25 39.5833 43.25H10.4167C8.40114 43.25 6.75 41.5989 6.75 39.5833V10.4167C6.75 8.40114 8.40114 6.75 10.4167 6.75ZM13 17.3493V13H17.3288C17.0956 15.2866 15.281 17.114 13 17.3493ZM21.9244 13H24.4898C24.2348 19.2236 19.2407 24.2346 13 24.4898V21.9244C17.8155 21.6721 21.6723 17.7969 21.9244 13Z" stroke="#607D8B"/>
                </svg>
              </div>
              <div class="satellite-id text-sm text-center">
                <slot name="satellite-id">1</slot>
              </div>
              <div class="satellite-strength text-sm text-center">
                <slot name="satellite-strength">00%</slot>
              </div>
            </div>
</template>
