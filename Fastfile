# Fastfile

default_platform(:ios)

platform :ios do
  desc "Authenticate with Apple Developer Portal"
  lane :authenticate do
    match(type: "development")
  end

  desc "Build and test the app"
  lane :build_and_test do
    match(type: "development") # Ensure you have match configured for provisioning profiles
    build_app(scheme: "GimigoTheGecko", export_method: "development")
    scan(scheme: "GimigoTheGecko", device: "iPhone 12")
  end
end

