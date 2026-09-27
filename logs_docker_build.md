(level-5) (base) cool@Macintosh 2026_07_26_Day2 % docker build -t loan-approval-app .
[+] Building 80.1s (11/11) FINISHED                                                     docker:desktop-linux
 => [internal] load build definition from Dockerfile                                                    0.0s
 => => transferring dockerfile: 378B                                                                    0.0s
 => [internal] load metadata for docker.io/library/python:3.11-slim                                     3.1s
 => [internal] load .dockerignore                                                                       0.0s
 => => transferring context: 151B                                                                       0.0s
 => [1/6] FROM docker.io/library/python:3.11-slim@sha256:e41613d42d4891e4930f79523f93f81bbc7632584ec6  11.1s
 => => resolve docker.io/library/python:3.11-slim@sha256:e41613d42d4891e4930f79523f93f81bbc7632584ec65  0.0s
 => => sha256:88a70807275990e242dca8d17d20a7b42c4af240ec374fd7fb87867753df1890 249B / 249B              0.3s
 => => sha256:03f370686e3a4cbdd79e1271eb1040ed2b17cf85041be7905256e33daedbfc95 1.28MB / 1.28MB          1.9s
 => => sha256:a16ecc1c5e5e0d6330aa463bb21f817d14b4b22edf2993216897170dd06764f8 14.41MB / 14.41MB        4.2s
 => => sha256:bd36565c0fdebaf0f3af5c3b4ce610ca085ced32e9e9da850d95912f5f18f47b 30.19MB / 30.19MB       10.4s
 => => extracting sha256:bd36565c0fdebaf0f3af5c3b4ce610ca085ced32e9e9da850d95912f5f18f47b               0.4s
 => => extracting sha256:03f370686e3a4cbdd79e1271eb1040ed2b17cf85041be7905256e33daedbfc95               0.0s
 => => extracting sha256:a16ecc1c5e5e0d6330aa463bb21f817d14b4b22edf2993216897170dd06764f8               0.2s
 => => extracting sha256:88a70807275990e242dca8d17d20a7b42c4af240ec374fd7fb87867753df1890               0.0s
 => [internal] load build context                                                                       0.1s
 => => transferring context: 4.78MB                                                                     0.0s
 => [2/6] WORKDIR /app                                                                                  0.2s
 => [3/6] COPY requirements.txt .                                                                       0.0s
 => [4/6] RUN pip install     --no-cache-dir     -r requirements.txt                                   51.3s
 => [5/6] COPY . .                                                                                      0.1s
 => [6/6] RUN chmod +x start.sh                                                                         0.1s
 => exporting to image                                                                                 14.1s
 => => exporting layers                                                                                11.7s
 => => exporting manifest sha256:9bfbc6a3fe48824173bc55cd6fabd9daaf28d9e615c6b4ed4cbeb889af8ea5f5       0.0s
 => => exporting config sha256:eda015164bd8e7c4988f750d597285406958702be2677f40160b453c7d1d5dea         0.0s
 => => exporting attestation manifest sha256:b03eed09062865411daa5b88dafe59bdce32e10f8530812a510c0ef96  0.0s
 => => exporting manifest list sha256:78ff5ca16b036015fd983ec28350a385a217b9a29ee07c410db628b0f51e1f19  0.0s
 => => naming to docker.io/library/loan-approval-app:latest                                             0.0s
 => => unpacking to docker.io/library/loan-approval-app:latest                                          2.4s

View build details: docker-desktop://dashboard/build/desktop-linux/desktop-linux/53z9124jc5pvwir5uxyvtf6t7