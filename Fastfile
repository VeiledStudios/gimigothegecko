# Fastfile

default_platform(:ios)

platform :ios do
  desc "Build and test the app"
  lane :build_and_test do
    match(type: "development") # Ensure you have match configured for provisioning profiles
    build_app(scheme: "GimigoTheGecko", export_method: "development")
    scan(scheme: "GimigoTheGecko", device: "iPhone 12")
  end
end

