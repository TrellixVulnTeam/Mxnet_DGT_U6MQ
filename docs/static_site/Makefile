# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
#   http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing,
# software distributed under the License is distributed on an
# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
# KIND, either express or implied.  See the License for the
# specific language governing permissions and limitations
# under the License.

all: html

html:
	mkdir -p build
	wget -O src/assets/js/jquery-3.3.1.min.js https://code.jquery.com/jquery-3.3.1.min.js
	cd src && bundle install && JEKYLL_ENV=production bundle exec jekyll build --config _config_prod.yml -d ../build/html && cd ..


clean:
	rm -rf build
