import { useState, useRef, useEffect } from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { motion } from "framer-motion";
import { Heart, ArrowRight, ArrowLeft, Play, Pause, Volume2, VolumeX } from "lucide-react";

export default function GiftCard() {
  const slides = [
    {
      title: "Hai Sayang ❤️",
      message: " Terima kasih yaaa untuk jalan jalannya hari inii".",
    },
    {
      title: "Selamat! 🎉",
      message: "Selamat atas semua pencapaian kamuuu, SELAMAT JUGAA KAMU UDAH JADI PRADANA. YEAYYY!!!!. Aku bener-bener bangga banget sama kamu!",
    },
    {
      title: "Terima Kasih 💫",
      message: "Makasiii kamu sudah hadir di dunia iniiii dan menjadi majell yang super duper kemrennn. makasiii jugaaaa atas segala hal yang kamu kasih ke akuuu.",
    },
    {
      title: "I Love You 💕",
      message: "Semoga segala impian kamu terwujud.Tetapp semangatt yaa sayanggg i love youuu.Inget aku terus yaaaa",
    },
  ];

  const [index, setIndex] = useState(0);
  const [isPlaying, setIsPlaying] = useState(false);
  const [muted, setMuted] = useState(false);
  const [volume, setVolume] = useState(0.6);
  const audioRef = useRef<https://vt.tiktok.com/ZSD6SABWt/ | null>(null);
