import SwiftUI

@main
struct GolfLaunchMonitorApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
    }
}

struct ContentView: View {
    @State private var ballSpeed: Double = 0.0
    @State private var launchAngle: Double = 0.0

    var body: some View {
        VStack(spacing: 20) {
            Text("Golf Launch Monitor")
                .font(.largeTitle)
                .bold()

            Text("Ball Speed: \(String(format: "%.1f", ballSpeed)) m/s")
                .font(.title2)

            Text("Launch Angle: \(String(format: "%.1f", launchAngle))°")
                .font(.title2)

            Spacer()

            Button("Simulate Shot") {
                simulateShot()
            }
            .padding()
            .background(Color.green)
            .foregroundColor(.white)
            .cornerRadius(12)

            Spacer()
        }
        .padding()
    }

    func simulateShot() {
        // Random mock values for now
        ballSpeed = Double.random(in: 30...80)
        launchAngle = Double.random(in: 5...20)
    }
}
