WebP Express 0.15.3. Conversion triggered using bulk conversion, 2019-09-24 05:02:41

*WebP Convert 2.1.4*  ignited.
- PHP version: 7.3.1
- Server software: Apache

Stack converter ignited

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2015/08/image4xxl-11.jpg
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image4xxl-11.jpg.webp
- log-call-arguments: true
- converters: (array of 9 items)

The following options have not been explicitly set, so using the following defaults:
- converter-options: (empty array)
- shuffle: false
- preferred-converters: (empty array)
- extra-converters: (empty array)

The following options were supplied and are passed on to the converters in the stack:
- default-quality: 70
- encoding: "auto"
- max-quality: 80
- metadata: "none"
- near-lossless: 60
- quality: "auto"
------------


*Trying: cwebp* 

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2015/08/image4xxl-11.jpg
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image4xxl-11.jpg.webp
- default-quality: 70
- encoding: "auto"
- low-memory: true
- log-call-arguments: true
- max-quality: 80
- metadata: "none"
- method: 6
- near-lossless: 60
- quality: "auto"
- use-nice: true
- command-line-options: ""
- try-common-system-paths: true
- try-supplied-binary-for-os: true

The following options have not been explicitly set, so using the following defaults:
- alpha-quality: 85
- auto-filter: false
- preset: "none"
- size-in-percentage: null (not set)
- skip: false
- rel-path-to-precompiled-binaries: *****
------------

Encoding is set to auto - converting to both lossless and lossy and selecting the smallest file

Converting to lossy
Locating cwebp binaries
1 cwebp binaries found in common system locations
Checking if we have a supplied binary for OS: Darwin... We do.
We in fact have 1
A total of 2 cwebp binaries where found
Detecting versions of the cwebp binaries found (and verifying that they can be executed in the process)
Executing: /usr/local/bin/cwebp -version. Result: version: 1.0.3
Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12 -version
Exec failed (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12)
Trying executing the cwebs found until success. Starting with the ones with highest version number.
Creating command line options for version: 1.0.3
Quality of source is 100. This is higher than max-quality, so using max-quality instead (80)
The near-lossless option ignored for lossy
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 80 -alpha_q '85' -m 6 -low_memory '[doc-root]/wp-content/uploads/2015/08/image4xxl-11.jpg' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image4xxl-11.jpg.webp.lossy.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image4xxl-11.jpg.webp.lossy.webp'
File:      [doc-root]/wp-content/uploads/2015/08/image4xxl-11.jpg
Dimension: 870 x 1110
Output:    22650 bytes Y-U-V-All-PSNR 45.40 50.83 51.26   46.61 dB
           (0.19 bpp)
block count:  intra4:        915  (23.77%)
              intra16:      2935  (76.23%)
              skipped:      2120  (55.06%)
bytes used:  header:            216  (1.0%)
             mode-partition:   5039  (22.2%)
 Residuals bytes  |segment 1|segment 2|segment 3|segment 4|  total
  intra4-coeffs:  |   12676 |     183 |     164 |     126 |   13149  (58.1%)
 intra16-coeffs:  |     320 |     178 |     193 |     781 |    1472  (6.5%)
  chroma coeffs:  |    2056 |      91 |      73 |     526 |    2746  (12.1%)
    macroblocks:  |      18%|       2%|       3%|      77%|    3850
      quantizer:  |      27 |      26 |      21 |      16 |
   filter level:  |      42 |      11 |      28 |       7 |
------------------+---------+---------+---------+---------+-----------------
 segments total:  |   15052 |     452 |     430 |    1433 |   17367  (76.7%)

Success
Reduction: 90% (went from 225 kb to 22 kb)

Converting to lossless
Locating cwebp binaries
1 cwebp binaries found in common system locations
Checking if we have a supplied binary for OS: Darwin... We do.
We in fact have 1
A total of 2 cwebp binaries where found
Detecting versions of the cwebp binaries found (and verifying that they can be executed in the process)
Executing: /usr/local/bin/cwebp -version. Result: version: 1.0.3
Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12 -version
Exec failed (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12)
Trying executing the cwebs found until success. Starting with the ones with highest version number.
Creating command line options for version: 1.0.3
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 80 -alpha_q '85' -near_lossless 60 -m 6 -low_memory '[doc-root]/wp-content/uploads/2015/08/image4xxl-11.jpg' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image4xxl-11.jpg.webp.lossless.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image4xxl-11.jpg.webp.lossless.webp'
File:      [doc-root]/wp-content/uploads/2015/08/image4xxl-11.jpg
Dimension: 870 x 1110
Output:    229558 bytes (1.90 bpp)
Lossless-ARGB compressed size: 229558 bytes
  * Header size: 4653 bytes, image data size: 224879
  * Lossless features used: PREDICTION CROSS-COLOR-TRANSFORM SUBTRACT-GREEN
  * Precision Bits: histogram=5 transform=4 cache=10

Success
Reduction: 0% (went from 225 kb to 224 kb)

Picking lossy
cwebp succeeded :)

Converted image in 1284 ms, reducing file size with 90% (went from 225 kb to 22 kb)
