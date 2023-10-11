FROM ruby:3.0.2-alpine AS builder
RUN apk add \
    build-base \
    mariadb-dev
COPY Gemfile* .
RUN bundle install
FROM ruby:3.0.2-alpine AS runner
RUN apk add \
    tzdata \
    nodejs \
    curl \
    bash \
    npm \
    mariadb-dev
WORKDIR /app
# We copy over the entire gems directory for our builder image, containing the already built artifact
COPY --from=builder /usr/local/bundle/ /usr/local/bundle/
COPY . .
EXPOSE 3000
RUN npm install -g yarn
RUN rails webpacker:install
CMD ["rails", "server","-b", "0.0.0.0"]