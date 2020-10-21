pipeline {
    agent { docker { image 'triangulumlabs/buildpack:linux' } }
    stages {
        stage('pack') {
            parallel {
                stage('armel') {
                    steps {
                        sh 'sudo apt-get -qq install -y --no-install-recommends \
                            zlib1g-dev \
                            zlib1g-dev:arm64 \
                            zlib1g-dev:armel \
                            zlib1g-dev:armhf \
                            zlib1g-dev:i386 \
                            zlib1g-dev:mipsel \
                            zlib1g-dev:mips64el \
                            zlib1g-dev:ppc64el \
                            zlib1g-dev:s390x'
                        sh 'CONFIG_SITE=/etc/dpkg-cross/cross-config.amd64  DEB_BUILD_OPTIONS=nocheck dpkg-buildpackage -aarmel -Pcross,nocheck'
                    }
                }
                stage('armhf') {
                    steps {
                        sh 'sudo apt-get -qq install -y --no-install-recommends \
                            zlib1g-dev \
                            zlib1g-dev:arm64 \
                            zlib1g-dev:armel \
                            zlib1g-dev:armhf \
                            zlib1g-dev:i386 \
                            zlib1g-dev:mipsel \
                            zlib1g-dev:mips64el \
                            zlib1g-dev:ppc64el \
                            zlib1g-dev:s390x'
                        sh 'CONFIG_SITE=/etc/dpkg-cross/cross-config.amd64  DEB_BUILD_OPTIONS=nocheck dpkg-buildpackage -aarmhf -Pcross,nocheck'
                    }
                }
                stage('arm64') {
                    steps {
                        sh 'sudo apt-get -qq install -y --no-install-recommends \
                            zlib1g-dev \
                            zlib1g-dev:arm64 \
                            zlib1g-dev:armel \
                            zlib1g-dev:armhf \
                            zlib1g-dev:i386 \
                            zlib1g-dev:mipsel \
                            zlib1g-dev:mips64el \
                            zlib1g-dev:ppc64el \
                            zlib1g-dev:s390x'
                        sh 'CONFIG_SITE=/etc/dpkg-cross/cross-config.amd64  DEB_BUILD_OPTIONS=nocheck dpkg-buildpackage -aarm64 -Pcross,nocheck'
                    }
                }
                stage('i386') {
                    steps {
                        sh 'sudo apt-get -qq install -y --no-install-recommends \
                            zlib1g-dev \
                            zlib1g-dev:arm64 \
                            zlib1g-dev:armel \
                            zlib1g-dev:armhf \
                            zlib1g-dev:i386 \
                            zlib1g-dev:mipsel \
                            zlib1g-dev:mips64el \
                            zlib1g-dev:ppc64el \
                            zlib1g-dev:s390x'
                        sh 'CONFIG_SITE=/etc/dpkg-cross/cross-config.amd64  DEB_BUILD_OPTIONS=nocheck dpkg-buildpackage -ai386 -Pcross,nocheck'
                    }
                }
                stage('amd64') {
                    steps {
                        sh 'sudo apt-get -qq install -y --no-install-recommends \
                            zlib1g-dev \
                            zlib1g-dev:arm64 \
                            zlib1g-dev:armel \
                            zlib1g-dev:armhf \
                            zlib1g-dev:i386 \
                            zlib1g-dev:mipsel \
                            zlib1g-dev:mips64el \
                            zlib1g-dev:ppc64el \
                            zlib1g-dev:s390x'
                        sh 'CONFIG_SITE=/etc/dpkg-cross/cross-config.amd64  DEB_BUILD_OPTIONS=nocheck dpkg-buildpackage -aamd64 -Pcross,nocheck'
                    }
                }
                stage('mipsel') {
                    steps {
                        sh 'sudo apt-get -qq install -y --no-install-recommends \
                            zlib1g-dev \
                            zlib1g-dev:arm64 \
                            zlib1g-dev:armel \
                            zlib1g-dev:armhf \
                            zlib1g-dev:i386 \
                            zlib1g-dev:mipsel \
                            zlib1g-dev:mips64el \
                            zlib1g-dev:ppc64el \
                            zlib1g-dev:s390x'
                        sh 'CONFIG_SITE=/etc/dpkg-cross/cross-config.amd64  DEB_BUILD_OPTIONS=nocheck dpkg-buildpackage -amipsel -Pcross,nocheck'
                    }
                }
                stage('mips64el') {
                    steps {
                        sh 'sudo apt-get -qq install -y --no-install-recommends \
                            zlib1g-dev \
                            zlib1g-dev:arm64 \
                            zlib1g-dev:armel \
                            zlib1g-dev:armhf \
                            zlib1g-dev:i386 \
                            zlib1g-dev:mipsel \
                            zlib1g-dev:mips64el \
                            zlib1g-dev:ppc64el \
                            zlib1g-dev:s390x'
                        sh 'CONFIG_SITE=/etc/dpkg-cross/cross-config.amd64  DEB_BUILD_OPTIONS=nocheck dpkg-buildpackage -amips64el -Pcross,nocheck'
                    }
                }
                stage('ppc64el') {
                    steps {
                        sh 'sudo apt-get -qq install -y --no-install-recommends \
                            zlib1g-dev \
                            zlib1g-dev:arm64 \
                            zlib1g-dev:armel \
                            zlib1g-dev:armhf \
                            zlib1g-dev:i386 \
                            zlib1g-dev:mipsel \
                            zlib1g-dev:mips64el \
                            zlib1g-dev:ppc64el \
                            zlib1g-dev:s390x'
                        sh 'CONFIG_SITE=/etc/dpkg-cross/cross-config.amd64  DEB_BUILD_OPTIONS=nocheck dpkg-buildpackage -appc64el -Pcross,nocheck'
                    }
                }
                stage('s390x') {
                    steps {
                        sh 'sudo apt-get -qq install -y --no-install-recommends \
                            zlib1g-dev \
                            zlib1g-dev:arm64 \
                            zlib1g-dev:armel \
                            zlib1g-dev:armhf \
                            zlib1g-dev:i386 \
                            zlib1g-dev:mipsel \
                            zlib1g-dev:mips64el \
                            zlib1g-dev:ppc64el \
                            zlib1g-dev:s390x'
                        sh 'CONFIG_SITE=/etc/dpkg-cross/cross-config.amd64  DEB_BUILD_OPTIONS=nocheck dpkg-buildpackage -as390x -Pcross,nocheck'
                    }
                }
            }

        }
    }
}