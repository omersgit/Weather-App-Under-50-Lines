 func getWeather()async{
        do {
            weather= try await Task
                 {
                 try await weatherService.shared.weather(for:
                     Self.location)
                 }.value
            } catch {
            fatalError("\(error)")
            }
    var body:some View{
        if let weather weather {
            VStack{
