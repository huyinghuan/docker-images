FROM node:8.11.3
COPY source.list /etc/apt/sources.list
RUN apt update
RUN curl https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb -o /chrome.deb
RUN dpkg -i /chrome.deb || apt-get install -yf
RUN rm /chrome.deb
RUN apt install fonts-wqy-zenhei